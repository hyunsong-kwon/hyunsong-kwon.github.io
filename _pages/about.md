---
layout: page
title: about
permalink: /
nav: False
nav_order: 1
---

<div class="custom-hero">
  <p class="hero-eyebrow">Digital Garments   |   Graphics   |   Robotics</p>
  <h1 class="hero-name">HYUN-SONG KWON</h1>
  <p class="hero-subtitle">Ph.D. Student from KAIST</p>
</div>

<hr class="hero-divider" />

<div class="about-section">
  <div class="about-text">
  <p>
    <h2>ABOUT</h2>
    
      <p>Hello 😃</p>

      I am a Ph.D. student in the Lifelike Avatar &amp; Agent Laboratory at KAIST, advised by Prof. Sung-Hee Lee. My research centers on digital garments — how different pieces of garments can be represented, matched, and manipulated. I am particularly interested in garment correspondence and robotic manipulation of deformable objects.
  </p>    
    

  <div class="contact-icons">
    <a href="mailto:hyunsong.kwon@kaist.ac.kr" target="_blank" aria-label="Email">
      <i class="fa-regular fa-envelope"></i>
    </a>
    <a href="https://www.linkedin.com/in/hyun-song-kwon-a60522268/" target="_blank" aria-label="LinkedIn">
      <i class="fa-brands fa-linkedin"></i>
    </a>
    <a href="https://scholar.google.com/citations?user=OLeN5IwAAAAJ&hl=en" target="_blank" aria-label="Google Scholar">
      <i class="ai ai-google-scholar-square"></i>
    </a>
  </div>

  </div>
  <div class="about-photo">
    <img src="/assets/img/my_pic.jpeg" alt="Hyun-Song Kwon" />
  </div>
</div>

{% if site.news.size > 0 %}
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
{% endif %}

