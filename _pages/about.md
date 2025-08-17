---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<!-- ===== Introduction ===== -->
<div class="about-wrap">
  <div class="about-left">
    <h2>Introduction</h2>
    <p>
      I am <strong>Yifei Chen (陈逸飞)</strong>, a first-year M.S. student in Mechanical Engineering at Northwestern University, specializing in robotics and advised by <strong>Prof. Kevin M. Lynch</strong>. I received my B.Eng. in Robotics Engineering in 2024, where my undergraduate advisor was <strong>Prof. Hongqiang Wang</strong>.  
    </p>
    <p>
      In 2023, I worked as a visiting research assistant at the University of Wisconsin–Madison, advised by <strong>Prof. Xiaobin Xiong</strong> and <strong>Dr. Michael Wehner</strong>.  
    </p>
    <p>
      My research interests include dexterous manipulation, reinforcement learning, optimal control, real-time embedded systems, and humaniod robot of course.
    </p>
  </div>

  <div class="about-right">
    <h3>Education & Research</h3>
    <ul class="fact-list">
      <li>M.S. in Mechanical Engineering, Northwestern University</li>
      <li>Advisor: Kevin M. Lynch</li>
      <li>Visiting RA, UW–Madison</li>
      <li>B.Eng. in Robotics Engineering, 2024</li>
    </ul>

    <h3>Personal Interests</h3>
    <ul class="fact-list">
      <li>Popping Dance</li>
      <li>Snowboarding</li>
      <li>Running</li>
      <li>Travel</li>
    </ul>
  </div>
</div>

<hr/>

<!-- ===== Humanoid Robot Showcase ===== -->
<h2>Humanoid Robots in Daily Life</h2>
<p class="subtle">Some demos I explored for humanoid robots in everyday scenarios.</p>

<div class="media-grid">
  <figure class="video-card">
    <div class="video-wrap">
      <video controls autoplay muted loop playsinline>
        <source src="/videos/Restruant_service.mp4" type="video/mp4">
      </video>
    </div>
    <figcaption>Restaurant service interaction</figcaption>
  </figure>

  <figure class="video-card">
    <div class="video-wrap">
      <video controls autoplay muted loop playsinline>
        <source src="/videos/understanding_cmd.mp4" type="video/mp4">
      </video>
    </div>
    <figcaption>Command understanding and execution</figcaption>
  </figure>
</div>

<hr/>

<!-- ===== Photo Gallery ===== -->
<h2>Gallery</h2>
<p class="subtle">Snapshots from my research and daily life.</p>

<div class="gallery-grid">
  <img src="/images/dexnex_real.png" alt="Dexterous manipulation project">
  <img src="/images/Robosoft.JPG" alt="Robosoft Conference">
  <img src="/images/Presentation.JPG" alt="Conference Presentation">
  <img src="/images/Back_snow.JPG" alt="Snowboarding - Back view">
  <img src="/images/font_snow.JPG" alt="Snowboarding - Front view">
</div>

<!-- ===== Styling ===== -->
<style>
/* Layout */
.about-wrap {
  display: grid;
  grid-template-columns: 1.2fr 0.8fr;
  gap: 24px;
  align-items: start;
}
.about-left p { margin: 0 0 10px; }

/* Info Blocks */
.about-right h3 {
  margin: 12px 0 8px;
  font-size: 1.05rem;
}
.fact-list {
  list-style: none;
  padding: 0;
  margin: 0 0 12px 0;
}
.fact-list li {
  padding: 6px 10px;
  border: 1px solid #e6e6e6;
  border-radius: 10px;
  font-size: 0.95rem;
  margin-bottom: 6px;
}

/* Subtle text */
.subtle {
  color: #666;
  font-size: 0.95rem;
  margin-top: -8px;
}

/* Videos */
.media-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
  margin: 8px 0 0;
}
.video-card {
  margin: 0;
}
.video-wrap {
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 9;
  background: #000;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 14px rgba(0,0,0,0.06);
}
.video-wrap video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.video-card figcaption {
  font-size: 0.9rem;
  color: #555;
  margin-top: 6px;
}

/* Gallery */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(5, minmax(0, 1fr));
  gap: 10px;
  margin-top: 8px;
}
.gallery-grid img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}

/* Responsive */
@media (max-width: 900px) {
  .about-wrap { grid-template-columns: 1fr; }
  .media-grid { grid-template-columns: 1fr; }
  .gallery-grid { grid-template-columns: repeat(3, 1fr); }
}
@media (max-width: 560px) {
  .gallery-grid { grid-template-columns: repeat(2, 1fr); }
  .gallery-grid img { height: 150px; }
}
</style>
