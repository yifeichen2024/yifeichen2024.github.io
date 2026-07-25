---
permalink: /
title: "About Me"
hide_title: true
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="home-page">
  <section class="home-hero">
    <div>
      <p class="home-kicker">Robotics · Dexterous Manipulation · Humanoids</p>
      <h1 class="home-title">Yifei Chen (陈逸飞)</h1>
      <p class="home-lede">
        I am a first-year M.S. student in Mechanical Engineering at Northwestern University, specializing in robotics and advised by <strong>Prof. Kevin M. Lynch</strong>. I received my B.Eng. in Robotics Engineering in 2024, where my undergraduate advisor was <strong>Prof. Hongqiang Wang</strong>.
      </p>
      <p>
        In 2023, I worked as a visiting research assistant at the University of Wisconsin-Madison, advised by <strong>Prof. Xiaobin Xiong</strong> and <strong>Dr. Michael Wehner</strong>. My research interests include dexterous manipulation, reinforcement learning, optimal control, real-time embedded systems, and humanoid robots.
      </p>
      <ul class="home-focus" aria-label="Research focus">
        <li>Dexterous manipulation</li>
        <li>Reinforcement learning</li>
        <li>Optimal control</li>
        <li>Embedded systems</li>
        <li>Humanoid robots</li>
      </ul>
    </div>

    <aside class="home-panel" aria-label="Profile highlights">
      <div class="home-panel__header">
        <h2 class="home-panel__title">Profile</h2>
      </div>
      <ul class="home-facts">
        <li>
          <strong>Current</strong>
          <span>M.S. in Mechanical Engineering, Northwestern University</span>
        </li>
        <li>
          <strong>Advisor</strong>
          <span>Prof. Kevin M. Lynch</span>
        </li>
        <li>
          <strong>Previous</strong>
          <span>Visiting RA at UW-Madison; B.Eng. in Robotics Engineering</span>
        </li>
        <li>
          <strong>Outside the lab</strong>
          <span>Popping dance, snowboarding, running, and travel</span>
        </li>
      </ul>
    </aside>
  </section>

  <section class="home-section" aria-labelledby="updates-heading">
    <div class="home-section__header">
      <div>
        <h2 id="updates-heading">Updates</h2>
        <p class="home-section__note">Recent news, papers, writing, and project milestones.</p>
      </div>
    </div>

    <div class="updates-list">
      {% assign updates = site.data.updates | sort: "date" | reverse %}
      {% for update in updates limit: 5 %}
        <article class="update-item">
          <div>
            <time class="update-date" datetime="{{ update.date | date: '%Y-%m-%d' }}">{{ update.date | date: "%b %Y" }}</time>
            {% if update.label %}<span class="update-label">{{ update.label }}</span>{% endif %}
          </div>
          <div>
            <h3>
              {% if update.url %}
                <a href="{{ update.url | relative_url }}">{{ update.title }}</a>
              {% else %}
                {{ update.title }}
              {% endif %}
            </h3>
            {% if update.description %}<p>{{ update.description }}</p>{% endif %}
          </div>
        </article>
      {% endfor %}
    </div>
  </section>

  <section class="home-section" aria-labelledby="robot-heading">
    <div class="home-section__header">
      <div>
        <h2 id="robot-heading">Humanoid Robots in Daily Life</h2>
        <p class="home-section__note">Demos exploring robot interaction, manipulation, and command following.</p>
      </div>
    </div>

    <div class="video-showcase">
      <figure class="video-card">
        <div class="video-wrap">
          <video controls autoplay muted loop playsinline>
            <source src="{{ '/videos/in_hand_manipulation.mp4' | relative_url }}" type="video/mp4">
          </video>
        </div>
        <figcaption>Ongoing stable in-hand manipulation under gravity and external disturbances.</figcaption>
      </figure>

      <figure class="video-card">
        <div class="video-wrap">
          <video controls autoplay muted loop playsinline>
            <source src="{{ '/videos/Restruant_service.mp4' | relative_url }}" type="video/mp4">
          </video>
        </div>
        <figcaption>Restaurant service interaction.</figcaption>
      </figure>

      <figure class="video-card">
        <div class="video-wrap">
          <video controls autoplay muted loop playsinline>
            <source src="{{ '/videos/understanding_cmd.mp4' | relative_url }}" type="video/mp4">
          </video>
        </div>
        <figcaption>Command understanding and execution.</figcaption>
      </figure>
    </div>
  </section>

  <section class="home-section" aria-labelledby="gallery-heading">
    <div class="home-section__header">
      <div>
        <h2 id="gallery-heading">Gallery</h2>
        <p class="home-section__note">Snapshots from research and daily life.</p>
      </div>
    </div>

    <div class="gallery-grid">
      <img src="{{ '/images/dexnex_real.png' | relative_url }}" alt="Dexterous manipulation project">
      <img src="{{ '/images/Robosoft.JPG' | relative_url }}" alt="Robosoft conference">
      <img src="{{ '/images/Presentation.JPG' | relative_url }}" alt="Conference presentation">
      <img src="{{ '/images/Back_snow.JPG' | relative_url }}" alt="Snowboarding back view">
      <img src="{{ '/images/font_snow.JPG' | relative_url }}" alt="Snowboarding front view">
    </div>
  </section>
</div>
