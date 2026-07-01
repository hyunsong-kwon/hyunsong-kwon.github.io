---
layout: page
title: about
permalink: /
nav: False
nav_order: 1
---

<div class="custom-hero">
  <p class="hero-eyebrow">RESEARCHER · DIGITAL GARMENTS</p>
  <h1 class="hero-name">HYUN-SONG KWON</h1>
  <p class="hero-subtitle">Ph.D. Student from KAIST. | Digital Garments · Graphics · Robotics</p>
</div>

<hr class="hero-divider" />

<div class="about-section">
  <div class="about-text">
    <h2>ABOUT</h2>
    <p>
      Hello 😃

      I am a Ph.D. student in the <a href="https://lava.kaist.ac.kr/">Lifelike Avatar &amp; Agent Laboratory</a> at KAIST, advised by Prof. Sung-Hee Lee. My research centers on digital garments — how different pieces of garments can be represented, matched, and manipulated. I am particularly interested in garment correspondence and robotic manipulation of deformable objects.
    </p>
  </div>
  <div class="about-photo">
    <img src="/assets/img/my_pic.jpeg" alt="Hyun-Song Kwon" />
  </div>
</div>

<div class="news-section">
  <h2>NEWS</h2>
  <div class="news-list">
    {% assign sorted_news = site.news | sort: 'date' | reverse %}
    {% for item in sorted_news limit:5 %}
    <div class="news-item">
      <div class="news-date">{{ item.date | date: "%b %-d, %Y" }}</div>
      <div class="news-content">{{ item.content }}</div>
    </div>
    {% endfor %}
  </div>
</div>

<div class="links-section">
  <h2>LINKS</h2>
  <div class="links-grid">
    <a href="https://github.com/사용자명" class="link-item" target="_blank">
      <span><span class="link-arrow">→</span> GITHUB</span>
      <i class="fa-brands fa-github"></i>
    </a>
    <a href="https://linkedin.com/in/사용자명" class="link-item" target="_blank">
      <span><span class="link-arrow">→</span> LINKEDIN</span>
      <i class="fa-brands fa-linkedin"></i>
    </a>
    <a href="mailto:본인이메일@kaist.ac.kr" class="link-item">
      <span><span class="link-arrow">→</span> EMAIL</span>
      <i class="fa-solid fa-envelope"></i>
    </a>
    <a href="https://lava.kaist.ac.kr/" class="link-item" target="_blank">
      <span><span class="link-arrow">→</span> LAB WEBPAGE</span>
      <i class="fa-solid fa-globe"></i>
    </a>
  </div>
</div>