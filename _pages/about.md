---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  dl {
    margin-bottom: 60px; /* 调整这个值以获得合适的间距 */
    clear: both;
  }

  /* 全局文本颜色 */
  body {
    color: #333; /* 主要文本颜色 */
    /* background-image: url('../images/bg.jpg'); 背景图片 */
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
  }

  /* 链接颜色 */
  a {
    color: #0066cc; /* 链接颜色 */
  }

  /* 作者名字颜色 */
  strong {
    color: #000; /* 作者名字颜色 */
  }

  /* 年份标题颜色 */
  .year-title {
    color: #666;
  }

  /* 会议标签样式 */
  .conference-label {
    position: absolute;
    top: 10px;
    left: -5px;
    background-color: #2c3e50;  /* 深蓝色背景 */
    color: white;  /* 白色文字 */
    padding: 6px 12px;
    border-radius: 6px;
    font-size: 0.95em;
    font-weight: 600;
    letter-spacing: 0.5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    z-index: 1;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-style: italic;  /* 添加斜体 */
  }

  /* 鼠标悬停效果 */
  .conference-label:hover {
    background-color: #34495e;  /* 悬停时稍微变亮 */
    transition: background-color 0.2s ease;
  }

  dl dt img {
    width: 100%; /* 在移动端默认占满宽度 */
    aspect-ratio: 2/1; /* 设置宽高比为2:1，即高度为宽度的一半 */
    object-fit: cover; /* 确保图片不会被裁剪 */
    display: block;
    margin: 10px 10px 10px 0px; /* 适当的间距 */
    
    /* 添加美化效果 */
    border-radius: 8px; /* 让图片有轻微的圆角 */
    border: 2px solid #ddd; /* 添加淡灰色的边框 */
    box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2); /* 添加轻微阴影 */
    padding: 5px; /* 给图片一些内边距，让它不贴着边框 */
    background-color: #fff; /* 设置背景色，让图片更加干净 */
  }

  /* 在桌面端（宽度大于768px）时固定宽度 */
  @media screen and (min-width: 768px) {
    dl dt img {
      width: 350px;
    }
  }

  dl dt {
    position: relative;
  }

  hr {
    border: 1px solid #ebebeb; /* 调整分隔线的颜色和样式 */
    /* margin: 10px;  */
    clear: both; 
  }

  dl dd {
  margin-top: 5px; 
  margin-bottom: 5px;
}

  dl dd strong {
  font-weight: bold;
  color: black;
  }

  .co-first {
    color: red;
  }

  .down {
    transform: rotate(180deg);
  }

  /* 教育和工作经历卡片样式 */
  .experience-card, .education-card {
    display: flex;
    align-items: center;
    gap: 25px;
    margin-bottom: 15px;
    padding: 20px;
    background: #f8f9fa;
    border-radius: 12px;
    transition: all 0.3s ease;
    border: 1px solid #e9ecef;
  }

  .experience-card:hover, .education-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    border-color: #dee2e6;
  }

  .experience-info, .education-info {
    flex: 1;
  }

  .experience-logo, .education-logo {
    flex-shrink: 0;
    width: 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: white;
    border-radius: 10px;
    padding: 10px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  }

  .experience-logo img, .education-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .experience-title, .education-title {
    font-size: 1.2em;
    margin-bottom: 8px;
    color: #2c3e50;
  }

  .experience-title a, .education-title a {
    color: #2c3e50;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .experience-title a:hover, .education-title a:hover {
    color: #3498db;
  }

  .experience-role, .education-role {
    color: #666;
    font-style: italic;
    margin-bottom: 5px;
  }

  .experience-topics, .education-topics {
    color: #666;
    font-style: italic;
  }

  .section-title {
    font-size: 1.8em;
    color: #2c3e50;
    margin: 40px 0 20px;
    padding-bottom: 10px;
    border-bottom: 2px solid #ecf0f1;
  }

  /* 奖学金和荣誉部分样式 */
  .honors-list {
    list-style: none;
    padding: 0;
  }

  .honors-list li {
    margin-bottom: 15px;
    padding: 15px 20px;
    background: #f8f9fa;
    border-radius: 8px;
    border-left: 4px solid #3498db;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .honors-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .honors-list li strong {
    color: #2c3e50;
  }

  .honors-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .honors-list li a:hover {
    color: #2980b9;
  }

  /* 服务部分样式 */
  .service-section {
    margin-bottom: 30px;
  }

  .service-section h3 {
    color: #2c3e50;
    font-size: 1.3em;
    margin: 25px 0 15px;
    padding-bottom: 8px;
    border-bottom: 2px solid #ecf0f1;
  }

  .service-list {
    list-style: none;
    padding: 0;
  }

  .service-list li {
    margin-bottom: 12px;
    padding: 12px 15px;
    background: #f8f9fa;
    border-radius: 6px;
    transition: transform 0.3s ease;
  }

  .service-list li:hover {
    transform: translateX(5px);
  }

  .service-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .service-list li a:hover {
    color: #2980b9;
  }

.hobbies-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 15px;
  margin-top: 15px;
}

.hobbies-gallery img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 3px 8px rgba(0,0,0,0.2);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.hobbies-gallery img:hover {
  transform: scale(1.03);
  box-shadow: 0 6px 16px rgba(0,0,0,0.3);
}

/* Force horizontal images into one row */
.wide-row {
  grid-column: 1 / -1; /* span full width of grid */
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 15px;
}


/* === Projects section === */
.projects-section {
  margin: 5px 0 0px;
}

.projects-title {
  font-size: 1.8em;
  color: #2c3e50;
  margin: 0 0 16px;
  padding-bottom: 0px;
  border-bottom: 2px solid #ecf0f1;
}

/* 2 columns on wide screens, 1 column on mobile */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
}

@media (max-width: 720px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
}

/* Card */
.project-card {
  background: #fff;
  border: 1px solid #e9ecef;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,.05);
  transition: transform .18s ease, box-shadow .18s ease, border-color .18s ease;
  display: flex;
  flex-direction: column;
}

.project-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 18px rgba(0,0,0,.08);
  border-color: #dee2e6;
}

.project-media {
  position: relative;
  width: 100%;
  aspect-ratio: 16 / 10;
  overflow: hidden;
  background: #fff; /* white background instead of grey */
}

.project-media img,
.project-media video {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: contain;     /* show full image */
  object-position: center; /* centerize horizontally & vertically */
  display: block;
}


/* Optional subtle zoom on hover for a lively feel */
.project-card:hover .project-media img,
.project-card:hover .project-media video {
  transform: scale(1.03);
  transition: transform .3s ease;
}

/* Title + actions */
.project-body {
  padding: 12px 14px 14px;
  display: grid;
  grid-template-columns: 1fr auto;
  align-items: center;
  gap: 10px;
}

.project-title {
  margin: 0;
  font-weight: 700;
  color: #2c3e50;
  font-size: 1.02rem;
  line-height: 1.3;
  letter-spacing: .2px;
}

/* GitHub button */
.project-gh {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 8px 12px;
  border-radius: 8px;
  border: 1px solid #e1e8f0;
  background: #f0f4f8;
  color: #2c3e50;
  text-decoration: none;
  font-weight: 600;
  font-size: .92rem;
  transition: background .18s ease, border-color .18s ease, transform .18s ease;
  white-space: nowrap;
}

.project-gh:hover {
  background: #eaf4ff;
  border-color: #9fb9d6;
  transform: translateY(-1px);
}

.project-gh svg {
  width: 18px; height: 18px;
  fill: currentColor;
  flex-shrink: 0;
}

/* ===== Publications (fixed + light) ===== */
.pub-card {
  display: grid;
  grid-template-columns: 320px 1fr;  /* a bit wider media column */
  gap: 18px;
  align-items: stretch;
  background: #fff;                  /* force light */
  border: 1px solid #e9ecef;
  border-radius: 14px;
  box-shadow: 0 2px 8px rgba(0,0,0,.05);
  padding: 14px;
  margin: 16px 0;
  transition: box-shadow .2s ease, transform .2s ease, border-color .2s ease;
  overflow: hidden;                  /* stop media bleed */
  box-sizing: border-box;
}
.pub-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 22px rgba(0,0,0,.08);
  border-color: #dee2e6;
}

/* Media column */
.pub-media {
  position: relative;     /* so badge can sit inside */
  width: 100%;
  border-radius: 10px;
  overflow: hidden;
  border: 1px solid #eef2f5;
  background: #fff;
  aspect-ratio: 16/10;
  box-sizing: border-box;
}
/* IMPORTANT: no absolute positioning; no hover-zoom */
.pub-media img,
.pub-media video {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: contain;               /* show full content */
  object-position: center;           /* center it */
}

/* Status badge */
.pub-badge {
  position: absolute;     /* pins it inside the pub-media box */
  top: 10px;
  left: 10px;
  background: #edf5ff;
  color: #1d4ed8;
  border: 1px solid #d6e6ff;
  font-size: .78rem;
  font-weight: 700;
  letter-spacing: .2px;
  padding: 6px 10px;
  border-radius: 999px;
  box-shadow: 0 1px 3px rgba(0,0,0,.06);
  z-index: 2;             /* make sure it sits above the image */
}
:root {
  --badge-bg: #edf5ff;
  --badge-fg: #1d4ed8;
  --badge-br: #d6e6ff;
}
.pub-badge,
.pub-badge.is-prep,
.pub-badge.is-progress {
  background: var(--badge-bg);
  color: var(--badge-fg);
  border-color: var(--badge-br);
}


/* Content */
.pub-body { display: grid; gap: 10px; align-content: start; }
.pub-title  { margin: 0; font-size: 1.05rem; line-height: 1.35; color: #2c3e50; font-weight: 800; }
.pub-authors{ margin: 0; color: #555; font-size: .98rem; }
.pub-affils { margin: 4px 0 0 0; color: #666; font-size: .9rem; }

/* Action chips */
.pub-actions { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 2px; }
.pub-chip {
  display: inline-flex; align-items: center; gap: 8px;
  padding: 6px 10px; border-radius: 8px;
  border: 1px solid #e1e8f0; background: #f7f9fc;
  color: #2c3e50; text-decoration: none; font-weight: 600; font-size: .9rem;
  transition: background .15s ease, border-color .15s ease, transform .15s ease;
}
.pub-chip:hover, .pub-chip:focus {
  background: #eaf4ff; border-color: #9fb9d6; transform: translateY(-1px);
  outline: none;
}
.pub-chip svg { width: 16px; height: 16px; fill: currentColor; }

/* Mobile */
@media (max-width: 820px) {
  .pub-card { grid-template-columns: 1fr; padding: 12px; }
  .pub-media { aspect-ratio: 16/9; }
}

/* If you previously added a dark-mode block for .pub-*, remove it.
   Otherwise, this forces light mode specifically for these cards. */

/* Hide projects 7+ until opened (prevents flash of visible content) */
.projects-grid:not(.is-open) .project-card:nth-of-type(n + 7) { 
  display: none !important; 
}

/* Button: full-width blue (keeps your previous styles) */
:root {
  --brand-blue: #1d4ed8;
  --brand-blue-weak: #edf5ff;
}
.load-more {
  grid-column: 1 / -1;
  justify-self: stretch;
  width: 100%;
  display: block;
  padding: 14px 18px;
  border-radius: 12px;
  border: 2px solid var(--brand-blue);
  background: #fff;
  color: var(--brand-blue);
  font-weight: 800;
  font-size: 1rem;
  text-align: center;
  cursor: pointer;
  transition: background .18s ease, border-color .18s ease, color .18s ease, transform .18s ease;
}
.load-more:hover { background: var(--brand-blue-weak); transform: translateY(-1px); }

/* Hide the button once opened (CSS-only) */
.projects-grid.is-open #loadMoreBtn { display: none !important; }

  .endorsements { display: grid; gap: 16px; margin: 12px 0 8px; }
  .endorse-card {
    background: #fff;
    border: 1px solid #e9ecef;
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(0,0,0,.05);
    padding: 14px;
  }
  .endorse-header {
    display: grid;
    grid-template-columns: 76px 1fr;
    gap: 12px;
    align-items: center;
  }
  .endorse-avatar {
    width: 76px; height: 76px;
    border-radius: 50%;
    overflow: hidden;
    border: 2px solid #ecf0f1;
    background: #fff;
  }
  .endorse-avatar img { width: 100%; height: 100%; object-fit: cover; }
  .endorse-name { margin: 0; font-weight: 800; color: #2c3e50; font-size: 1.02rem; }
  .endorse-affil { color: #666; font-size: .93rem; margin-top: 2px; }
  .endorse-links { display: flex; gap: 8px; margin-top: 6px; flex-wrap: wrap; }
  .endorse-links a {
    display: inline-flex; align-items: center; justify-content: center;
    width: 34px; height: 34px; border-radius: 8px;
    background: #f0f4f8; border: 1px solid #e1e8f0; text-decoration: none;
  }
  .endorse-links svg { width: 18px; height: 18px; fill: #2c3e50; }
  .endorse-quote {
    margin: 12px 2px 2px 2px;
    padding: 12px 14px;
    background: #f8f9fa;
    border-left: 4px solid #3498db;
    border-radius: 8px;
    color: #333;
    line-height: 1.55;
    font-style: italic;
  }
  @media (max-width: 480px) {
    .endorse-header { grid-template-columns: 64px 1fr; }
    .endorse-avatar { width: 64px; height: 64px; }
  }

  /* Vertical Endorsements */
  .endorsements { display: grid; gap: 16px; margin: 12px 0 8px; }
  .endorse-card {
    background: #fff;
    border: 1px solid #e9ecef;
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(0,0,0,.05);
    padding: 14px;
  }
  .endorse-header {
    display: grid;
    grid-template-columns: 76px 1fr;
    gap: 12px;
    align-items: center;
  }
  .endorse-avatar {
    width: 76px; height: 76px;
    border-radius: 50%;
    overflow: hidden;
    border: 2px solid #ecf0f1;
    background: #fff;
  }
  .endorse-avatar img { width: 100%; height: 100%; object-fit: cover; }
  .endorse-name { margin: 0; font-weight: 800; color: #2c3e50; font-size: 1.02rem; }
  .endorse-affil { color: #666; font-size: .93rem; margin-top: 2px; }
  .endorse-links { display: flex; gap: 8px; margin-top: 6px; flex-wrap: wrap; }
  .endorse-links a {
    display: inline-flex; align-items: center; justify-content: center;
    width: 34px; height: 34px; border-radius: 8px;
    background: #f0f4f8; border: 1px solid #e1e8f0; text-decoration: none;
    transition: background .18s ease, border-color .18s ease, transform .18s ease, box-shadow .18s ease;
  }
  .endorse-links svg { width: 18px; height: 18px; fill: #2c3e50; }
  .endorse-quote {
    margin: 12px 2px 2px 2px;
    padding: 12px 14px;
    background: #f8f9fa;
    border-left: 4px solid #3498db;
    border-radius: 8px;
    color: #333;
    line-height: 1.55;
    font-style: italic;
  }
  @media (max-width: 480px) {
    .endorse-header { grid-template-columns: 64px 1fr; }
    .endorse-avatar { width: 64px; height: 64px; }
  }

  /* Remove underlines for button-like links, keep them clean on hover */
  .pub-actions a,
  .pub-actions a:visited,
  .pub-chip,
  .pub-chip:visited,
  .project-gh,
  .project-gh:visited,
  .endorse-links a,
  .endorse-links a:visited {
    text-decoration: none !important;
    box-shadow: none !important;
    background-image: none !important;
  }
  .pub-actions a:hover,
  .pub-chip:hover,
  .project-gh:hover,
  .endorse-links a:hover,
  .endorse-links a:focus {
    text-decoration: none !important;
    box-shadow: none !important;
    background-image: none !important;
  }

  /* Pop hover for endorsement buttons to match other buttons */
  .endorse-links a:hover,
  .endorse-links a:focus {
    background: #eaf4ff;
    border-color: #9fb9d6;
    transform: translateY(-1px);
    box-shadow: 0 2px 8px rgba(0,0,0,.08);
  }

  /* Accessible focus ring */
  .endorse-links a:focus-visible,
  .project-gh:focus-visible,
  .pub-chip:focus-visible,
  .pub-actions a:focus-visible {
    outline: 2px solid #9fb9d6;
    outline-offset: 2px;
  }


/* Make project cards feel clickable */
.project-card.is-clickable { cursor: pointer; }
.project-card.is-clickable:focus {
  outline: 2px solid #9fb9d6;
  outline-offset: 3px;
}

  /* Education metrics chips */
  .edu-metrics {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 10px;
  }
  .chip, .chip-button {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 6px 10px;
    border-radius: 999px;
    border: 1px solid #e1e8f0;
    background: #f7f9fc;
    color: #2c3e50;
    font-weight: 700;
    font-size: .9rem;
    cursor: default;
    user-select: none;
  }
  .chip-button {
    cursor: pointer;
    transition: background .15s ease, border-color .15s ease, transform .15s ease;
  }
  .chip-button:hover, .chip-button:focus {
    background: #eaf4ff;
    border-color: #9fb9d6;
    transform: translateY(-1px);
    outline: none;
  }

  /* 4.0 courses list */
  .course-list {
    margin: 10px 0 0 0;
    padding: 12px 14px;
    background: #ffffff;
    border: 1px solid #e9ecef;
    border-radius: 10px;
    box-shadow: 0 2px 6px rgba(0,0,0,.05);
    list-style: none;
  }
  .course-list li {
    padding: 6px 2px;
    border-bottom: 1px dashed #e9ecef;
  }
  .course-list li:last-child { border-bottom: 0; }
  .is-hidden { display: none !important; }

  .course-list-inline {
    margin: 10px 0 0 0;
    padding: 12px 14px;
    background: #ffffff;
    border: 1px solid #e9ecef;
    border-radius: 10px;
    box-shadow: 0 2px 6px rgba(0,0,0,.05);
    line-height: 1.6;
    font-size: 0; /* prevent HTML whitespace between items */
  }
  .course-list-inline .course-item {
    display: inline;
    font-size: 1rem; /* restore readable size */
  }
  .course-list-inline .course-item + .course-item::before {
    content: ", ";
  }

  .course-list-inline {
  font-size: 0; /* prevent HTML whitespace */
  }
  .course-list-inline .course-item {
    display: inline;
    font-size: 1rem;
  }

</style>

<!-- {% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %} -->

<span class='anchor' id='about-me'></span>


# About Me  
I am **Shayan Kebriti**, a Computer Engineering undergraduate at Shahid Beheshti University in Tehran, Iran.  
My research interests include **Machine Learning**, **Computer Vision**, **Medical Image Computing**, and **Graph Neural Networks**.  
I am open to working on projects in these areas and I would love to contribute. I am also seeking **Master’s** or **PhD** opportunities.  

*Email:* [shayankebriti@gmail.com](mailto:shayankebriti@gmail.com)



# Publications
<div class="pub-card">
  <div class="pub-media">
    <span class="pub-badge">
      Under Review (
      <a href="https://www.scimagojr.com/journalsearch.php?q=17271&tip=sid" target="_blank">
        Medical Image Analysis
      </a>)
    </span>
    <img src="images/fractmorph.png" alt="FractMorph figure">
  </div>

  <div class="pub-body">
    <h3 class="pub-title">FractMorph: A Fractional Fourier-Based Multi-Domain Transformer for Deformable Image Registration</h3>

    <p class="pub-authors">
      <strong>Shayan Kebriti</strong><sup>1</sup>,
      Shahabedin Nabavi<sup>1</sup>
      <a href="https://scholar.google.com/citations?user=D_mPA6sAAAAJ" target="_blank" aria-label="Nabavi Google Scholar">
        🎓
      </a>,
      Ali Gooya<sup>2,3</sup>
      <a href="https://scholar.google.com/citations?user=H7w9icgAAAAJ" target="_blank" aria-label="Gooya Google Scholar">
        🎓
      </a>
    </p>

    <div class="pub-actions">
      <a class="pub-chip" href="https://arxiv.org/abs/2508.12445" target="_blank" rel="noopener">
        arXiv
      </a>
      <a class="pub-chip" href="https://arxiv.org/pdf/2508.12445" target="_blank" rel="noopener">
        Paper (PDF)
      </a>
      <a class="project-gh" href="https://github.com/shayankebriti/FractMorph" target="_blank" rel="noopener">
        <svg viewBox="0 0 16 16" aria-hidden="true">
          <path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/>
        </svg>
        GitHub
      </a>
    </div>

    <p class="pub-abstract">
      FractMorph is a novel 3D dual-parallel transformer for deformable image registration. Its Fractional Cross-Attention blends multi-scale spectral–spatial features via fractional Fourier transforms, achieving state-of-the-art results on <strong>intra-patient cardiac</strong> and <strong>atlas-to-patient cerebral</strong> MRI benchmarks.
    </p>

    <p class="pub-affils">
      <sup>1</sup> Faculty of Computer Science and Engineering, Shahid Beheshti University, Tehran, Iran<br>
      <sup>2</sup> School of Computing Science, University of Glasgow, Glasgow, UK<br>
      <sup>3</sup> Alan Turing Institute, London, UK
    </p>
  </div>
</div>





<div class="pub-card">
  <div class="pub-media">
    <span class="pub-badge is-prep">Manuscript in Preparation</span>
    <img src="images/perfusion.png" alt="Perfusion software overview">
  </div>

  <div class="pub-body">
    <h3 class="pub-title">Design and Implementation of a Software for Measurement of Brain Perfusion Using an Optimized Model</h3>

    <!-- Collaborators (text unchanged; just swapped GS icons for 🎓) -->
    <p>
      This work is carried out under the supervision of 
      Dr. Oghabian<sup>1,2</sup> 
      <a href="https://scholar.google.com/citations?user=yMK1nMcAAAAJ" target="_blank">🎓</a>
      <a href="http://www.oghabian.net/" target="_blank">🔗</a>,
      in collaboration with 
      Dr. Mohammadi<sup>1,2</sup> 
      <a href="https://scholar.google.com/citations?user=bHz_xXUAAAAJ" target="_blank">🎓</a>
      <a href="https://www.mdimohammadi.com/" target="_blank">🔗</a>,
      Dr. Irandoost<sup>1,2</sup> 
      <a href="https://www.linkedin.com/in/soheil-ahmadzadeh-irandoost-8391a397/" target="_blank">🔗</a> and 
      Dr. Zare<sup>1,2</sup> 
      <a href="https://www.linkedin.com/in/alale-zare-597442107/" target="_blank">🔗</a>
    </p>

    <!-- Expandable sections (unchanged text) -->
    <details class="pub-details" style="margin-top:0px;">
      <summary><strong>Project Description</strong></summary>
      <p>
        The NIAG perfusion software is developed for the quantitative analysis of brain perfusion MRI. 
        It supports standard medical image formats, provides preprocessing tools such as motion correction, 
        denoising, segmentation, and slice-time correction, and computes key DSC perfusion parameters 
        (<strong>CBF, CBV, MTT, AUC</strong>). 
        It also offers advanced visualization features like mirror-mode maps and customizable ROI definition 
        for detailed regional assessment of cerebral hemodynamics. 
        <strong>The software is intended for real clinical use in hospitals under the supervision of Tehran University 
        of Medical Sciences.</strong>
      </p>
    </details>

    <details class="pub-details">
      <summary><strong>My Contributions</strong></summary>
      <p>
        My current contributions have focused on enhancing the software’s analytical pipeline, including the 
        <strong>refinement of brain segmentation methods for complex tumor cases</strong>, improvements in 
        preprocessing routines, and extension of <strong>manual ROI handling and visualization modules</strong>. 
        I have also <strong>increased the quality and resolution of perfusion MRI images while ensuring precise 
        metric calculations</strong>, and carried out the <strong>implementation and debugging of perfusion 
        parameter calculations</strong>.
      </p>
    </details>

    <!-- Affiliations (unchanged text) -->
    <p class="pub-affils" style="margin-top:4px;">
      <sup>1</sup> Department of Medical Physics and Biomedical Engineering, School of Medicine, Tehran University of Medical Sciences, Tehran, Iran<br>
      <sup>2</sup> Neuroimaging and Analysis Group, Research Center for Molecular and Cellular Imaging, Advanced Medical Technologies and Equipment Institute, Tehran University of Medical Sciences, Tehran, Iran
    </p>
  </div>
</div>


## Bachelor Thesis

<div class="pub-card">
  <div class="pub-media">
    <span class="pub-badge is-progress">In Progress</span>
    <img src="images/bsc-thesis.png" alt="Anatomical mesh generation framework">
  </div>

  <div class="pub-body">
    <h3 class="pub-title">A Framework for Anatomical Mesh Generation From Medical Images for In-Silico Simulations</h3>

    <!-- (Text unchanged) -->
    <p class="pub-abstract">
      This ongoing work aims to develop a novel deep learning framework for anatomical mesh generation from medical images without requiring manual annotations. The framework consists of an anatomical structure <strong>segmentation network</strong>, <strong>a graph neural network for 3D mesh control-handle generation</strong>, and a <strong>deformation stage</strong> for final enhancements. The generated meshes are designed for use in in-silico simulations for <strong>multiple modalities</strong> such as <strong>CT</strong> and <strong>MR</strong> scans, enabling <strong>virtual experiments</strong> and <strong>computational modeling</strong> of anatomy for <strong>research</strong>, <strong>surgical planning</strong>, and <strong>medical device testing</strong>. More updates coming soon!
    </p>
  </div>
</div>


# Projects
You can browse a categorized list of my open-source projects <a href="https://github.com/shayankebriti" target="_blank" rel="noopener">on my Github profile</a>. Here is a selection of them:
<div class="projects-section">
  <div class="projects-grid">
    <!-- Project 1 -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/wgtd3.png" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Multi-Asset Trading with TD3 RL Agent and Wavelet-Coherence Graph Neural Networks</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/TD3-GNN-Multi-Asset-Trader" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 2 -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/diffusion-cifar10.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Conditional Diffusion with Simple and Attention-Based U-Nets for CIFAR-10 Image Generation</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Conditional-Diffusion-CIFAR10" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 3 -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/rock-paper.gif" alt="demo gif" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Rock–Paper–Scissors Automation with YOLOv11 and Cheat/Win Overlays</h3>
        <a class="project-gh" href="https://github.com/SBUformers/Rock-Paper-Scissors-Simulator" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 4 -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/hiv-gnn.png" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">HIV Inhibitors Classification with Multiple GNN Message Passing Methods</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/HIV-Inhibitors-Classification" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 5 -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/vae-gan.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Variational Autoencoder (VAE) Analysis & Denoising GAN</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Computer-Vision-assignments/tree/main/HW3" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 6 -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/multi-classification.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Fashion Product Multilabel Classification & Image-to-Text Title Generation Using RNNs</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Fashion-Product-Multilabel-Classification" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Load more trigger (appears after 6th project) -->
    <button id="loadMoreBtn" class="load-more" type="button" aria-expanded="false">
      Load more projects
    </button>

    <!-- Project 7 (hidden initially) -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/siamese.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Siamese Face Recognition Network Featuring A Graphical Web Interface</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Siamese-Face-Recognition" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 8 (hidden initially) -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/lord-of-the-coins.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">A puzzle-solving game implementing DFS, BFS, and A* search agents (designed as a TA assignment)</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Lord-of-the-Coins" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 9 (NEW, hidden initially) -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/compression-watermark.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Image Compressing & Watermarking Using Spatial and Spectral (DCT, DFT and DWT) Methods</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Computer-Vision-assignments/tree/main/HW0" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 10 (NEW, hidden initially) -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/classical-vision.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">Classical Image Processing & Non Local Means (NLM) Filter CPU and GPU Implementations</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/Computer-Vision-assignments/tree/main/HW1" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 11 (NEW, hidden initially) -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/rl.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">My Deep Reinforcement Learning Assignments</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/DRL-assignments" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>

    <!-- Project 12 (NEW, hidden initially) -->
    <article class="project-card">
      <div class="project-media">
        <img src="images/projects/ml.jpg" alt="demo" loading="lazy">
      </div>
      <div class="project-body">
        <h3 class="project-title">My Machine Learning Assignments</h3>
        <a class="project-gh" href="https://github.com/shayankebriti/ML-assignments" target="_blank" rel="noopener">
          <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M8 .2a8 8 0 0 0-2.53 15.6c.4.08.55-.17.55-.38l-.01-1.33c-2.25.49-2.72-1.09-2.72-1.09-.36-.93-.88-1.18-.88-1.18-.72-.5.05-.49.05-.49.79.06 1.2.83 1.2.83.71 1.2 1.86.85 2.31.65.07-.52.28-.85.5-1.05-1.8-.2-3.69-.9-3.69-3.98 0-.88.31-1.6.82-2.16-.08-.2-.36-1.01.08-2.11 0 0 .67-.22 2.2.82A7.7 7.7 0 0 1 8 3.87c.68 0 1.36.09 2 .26 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.28.82 2.16 0 3.1-1.9 3.78-3.71 3.98.29.25.54.73.54 1.48l-.01 2.2c0 .21.15.46.55.38A8 8 0 0 0 8 .2z"/></svg>
          GitHub
        </a>
      </div>
    </article>
  </div>
</div>

<script>
  (function () {
    const grid = document.querySelector('.projects-grid');
    const btn  = document.getElementById('loadMoreBtn');
    if (!grid || !btn) return;
    btn.addEventListener('click', () => {
      grid.classList.add('is-open');
      btn.setAttribute('aria-expanded', 'true');
    });
  })();
</script>

<script>
  (function () {
    // Make whole project cards clickable, using the href of the .project-gh button
    document.querySelectorAll('.projects-grid .project-card').forEach(card => {
      const gh = card.querySelector('.project-gh[href]');
      if (!gh) return; // skip cards with no GitHub link

      const url = gh.getAttribute('href');
      card.classList.add('is-clickable');
      card.setAttribute('role', 'link');

      // Improve screen reader label
      const title = card.querySelector('.project-title');
      if (title && !card.hasAttribute('aria-label')) {
        card.setAttribute('aria-label', `Open ${title.textContent.trim()} on GitHub`);
      }

      // Keyboard support
      card.tabIndex = 0;
      card.addEventListener('keydown', e => {
        if (e.target.closest('a, button')) return;
        if (e.key === 'Enter' || e.key === ' ') {
          e.preventDefault();
          window.open(url, '_blank', 'noopener');
        }
      });

      // Mouse or touch click, ignore clicks on existing links or buttons
      card.addEventListener('click', e => {
        if (e.target.closest('a, button')) return;
        window.open(url, '_blank', 'noopener');
      });
    });
  })();
</script>



# Education

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>Sep 2021 - Jan 2026</strong><br/>
      Bachelor, Computer Engineering, Shahid Beheshti Univeristy, Tehran, Iran
    </div>

    <div class="edu-metrics" aria-label="Education metrics">
      <span class="chip" title="Cumulative GPA">GPA: 3.86/4.00</span>
      <span class="chip" title="Last two academic years GPA">Last two years: 4.00/4.00</span>
    </div>

    <!-- Courses, names only, continuous with commas -->
    <div id="fourPointCourses" class="course-list-inline" role="list">
      <span style="font-size:1rem;"><strong>Relevant 4/4 Courses: </strong></span> 
      <span class="course-item" role="listitem">Computer Vision</span>
      <span class="course-item" role="listitem">Machine Learning</span>
      <span class="course-item" role="listitem">
      Deep RL (Graduate Course | <a href="docs/DRL-Seminar.pdf">My Seminar</a>)</span>
      <span class="course-item" role="listitem">Data Mining</span>
      <span class="course-item" role="listitem">Artificial Intelligence</span>
      <span class="course-item" role="listitem">Algorithms Design</span>
      <span class="course-item" role="listitem">Data Structures</span>
      <span class="course-item" role="listitem">Linear Algebra</span>
      <span class="course-item" role="listitem">Probability &amp; Statistics</span>
      <span class="course-item" role="listitem">Signal &amp; Systems</span>
      <span class="course-item" role="listitem">Fundamentals of Robotics</span>
    </div>



  </div>

  <div class="education-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
  </div>
</div>

<div class="education-card" aria-label="Education entry: Sampad Diploma in Mathematics and Physics">
  <div class="education-info">
    <div class="education-title">
      <strong>Sep 2019 – Jan 2021</strong><br/>
      Diploma, Mathematics & Physics, National Organization for Development of Exceptional Talents (Sampad), Iran
    </div>

    <div class="edu-metrics" aria-label="Education metrics">
      <span class="chip" title="Cumulative GPA">GPA: 4.00/4.00</span>
      <span class="chip" title="Ranked 1st in the school">Ranked 1st in the school</span>
    </div>
  </div>

  <div class="education-logo">
    <img src="../images/sampad.jfif" alt="National Organization for Development of Exceptional Talents (Sampad) logo" />
  </div>
</div>


# Experience

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      CNCH Competition
    </div>
    <div class="experience-role">Cognitive Neuroscience & AI Research Mentor</div>
    <div class="experience-topics">July 2025 - Now</div>
  </div>
  <div class="experience-logo">
    <img src="../images/CNCH.jpg" alt="Neuroscience Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://cniag.ir/en/">Neuroimaging and Analysis Group (NIAG), Tehran University of Medical Sciences</a>
    </div>
    <div class="experience-role">Medical Image Computing Engineer & Researcher</div>
    <div class="experience-topics">Nov 2024 - Now</div>
  </div>
  <div class="experience-logo">
    <img src="../images/TUMS.jfif" alt="Tehran University of Medical Sciences" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Shahid Beheshti University
    </div>
    <div class="experience-role">Undergraduate Researcher</div>
    <div class="experience-topics">June 2024 - Now</div>
  </div>
  <div class="experience-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Shahid Beheshti University
    </div>
    <div class="experience-role">Teaching Assistant (14 Courses)</div>
    <div class="experience-topics">Sep 2022 - Now</div>
  </div>
  <div class="experience-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Roshan AI
    </div>
    <div class="experience-role">ML Engineer & Data Scientist (Computer Vision and Trading Models)</div>
    <div class="experience-topics">Jul 2024 - Nov 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/roshan-ai.jfif" alt="Roshan AI logo" />
  </div>
</div>


<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://ipm.ac.ir/">Institute for Research in Fundamental Sciences (IPM)</a>
    </div>
    <div class="experience-role">AI Research Intern (Deep Learning for Perspective Transformation)</div>
    <div class="experience-topics">Jun 2024 - Aug 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/IPM.jpg" alt="IPM logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Collegiality UG (haftungsbeschränkt), Germany
    </div>
    <div class="experience-role">Software Developer</div>
    <div class="experience-topics">Sep 2022 - Dec 2023</div>
  </div>
  <div class="experience-logo">
    <img src="../images/Collegiality.jfif" alt="Collegiality logo" />
  </div>
</div>


# Endorsements
Here is what colleagues and supervisors have said about working with me:

<section class="endorsements" aria-label="Endorsements">
  <!-- Shahabedin FIRST -->
  <article class="endorse-card">
    <div class="endorse-header">
      <div class="endorse-avatar">
        <img src="images/shahabedin-nabavi.jfif" alt="Portrait of Shahabedin Nabavi">
      </div>
      <div class="endorse-meta">
        <h3 class="endorse-name">Shahabedin Nabavi, Ph.D. in Artificial Intelligence and Cognitive Computing</h3>
        <div class="endorse-affil">Shahid Beheshti University • Medical Image Analysis</div>
        <div class="endorse-links">
          <a href="https://www.linkedin.com/in/shahabedin-nabavi-32a38458/" target="_blank" rel="noopener" aria-label="LinkedIn, Shahabedin Nabavi" title="LinkedIn">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM.5 8h4V23h-4V8zm7.49 0h3.84v2.05h.06c.53-1 1.82-2.05 3.75-2.05 4.01 0 4.75 2.64 4.75 6.08V23h-4v-7.02c0-1.68-.03-3.85-2.35-3.85-2.35 0-2.71 1.84-2.71 3.73V23h-4V8z"/></svg>
          </a>
          <a href="https://scholar.google.com/citations?user=D_mPA6sAAAAJ" target="_blank" rel="noopener" aria-label="Google Scholar, Shahabedin Nabavi" title="Google Scholar">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M3 4a2 2 0 012-2h9a2 2 0 012 2v13a4 4 0 014 4H6a3 3 0 01-3-3V4zm13 0H5v14a1 1 0 001 1h12a2 2 0 00-2-2V4zM7 6h8v2H7V6zm0 4h8v2H7v-2zm0 4h6v2H7v-2z"/></svg>
          </a>
        </div>
      </div>
    </div>
    <blockquote class="endorse-quote">“It is my pleasure to strongly recommend Mr. Shayan Kebriti, one of my undergraduate students, for his exceptional academic performance, research contributions, and outstanding personal qualities.
I had the privilege of teaching Shayan in two courses: Computer Vision with Deep Learning, in which he achieved a perfect score of 20 out of 20, and Operating Systems Lab, where he ranked in the top 5% of the class. His performance in both courses demonstrated not only his deep understanding of the material but also his remarkable ability to apply theoretical concepts to practical challenges.
Beyond coursework, Shayan worked under my supervision on a research project in deformable image registration, which is currently under review in a reputable journal. His contributions to this work were significant, showing creativity, strong problem-solving skills, and a clear passion for advancing the field of artificial intelligence and medical image computing.
Shayan is a delighted, talented, and hardworking individual who consistently surprises me with his intellectual curiosity and eagerness to learn new concepts. He is particularly enthusiastic about exploring new developments in AI and medical imaging, a quality that makes him an ideal candidate for advanced research and professional growth. On a personal level, Shayan is polite, understanding, and highly reliable. His positive attitude, professionalism, and strong interpersonal skills make him a pleasure to work with, both in academic and research settings.<br>In summary, I have no doubt that Shayan will excel in any academic or professional environment he chooses to pursue. I wholeheartedly recommend him and am confident that he will make valuable contributions wherever he goes.”</blockquote>
  </article>

  <!-- Mahdi SECOND -->
  <article class="endorse-card">
    <div class="endorse-header">
      <div class="endorse-avatar">
        <img src="images/mahdi-mohammadi.jpg" alt="Portrait of Mohammadreza, Mahdi, Mohammadi">
      </div>
      <div class="endorse-meta">
        <h3 class="endorse-name">Mahdi Mohammadi, Ph.D. in Medical Physics</h3>
        <div class="endorse-affil">Tehran University of Medical Sciences • NIAG</div>
        <div class="endorse-links">
          <a href="https://www.linkedin.com/in/mahdi-mohammadi-98755717b/" target="_blank" rel="noopener" aria-label="LinkedIn, M. D. Mohammadi" title="LinkedIn">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM.5 8h4V23h-4V8zm7.49 0h3.84v2.05h.06c.53-1 1.82-2.05 3.75-2.05 4.01 0 4.75 2.64 4.75 6.08V23h-4v-7.02c0-1.68-.03-3.85-2.35-3.85-2.35 0-2.71 1.84-2.71 3.73V23h-4V8z"/></svg>
          </a>
          <a href="https://www.mdimohammadi.com" target="_blank" rel="noopener" aria-label="Website, M. D. Mohammadi" title="Website">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 2a10 10 0 100 20 10 10 0 000-20zm7.94 9h-3.11a15.9 15.9 0 00-1.3-5 8.01 8.01 0 014.41 5zM12 4c1.12 0 2.77 2.24 3.4 6H8.6C9.23 6.24 10.88 4 12 4zM6.47 6a15.9 15.9 0 00-1.3 5H2.06A8.01 8.01 0 016.47 6zM2.06 13h3.11c.16 1.77.64 3.5 1.3 5a8.01 8.01 0 01-4.41-5zm5.14 0h6.6c-.63 3.76-2.28 6-3.3 6s-2.67-2.24-3.3-6zm6.93 5a15.9 15.9 0 001.3-5h3.11a8.01 8.01 0 01-4.41 5z"/></svg>
          </a>
          <a href="https://scholar.google.com/citations?user=bHz_xXUAAAAJ" target="_blank" rel="noopener" aria-label="Google Scholar, M. D. Mohammadi" title="Google Scholar">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M3 4a2 2 0 012-2h9a2 2 0 012 2v13a4 4 0 014 4H6a3 3 0 01-3-3V4zm13 0H5v14a1 1 0 001 1h12a2 2 0 00-2-2V4zM7 6h8v2H7V6zm0 4h8v2H7v-2zm0 4h6v2H7v-2z"/></svg>
          </a>
        </div>
      </div>
    </div>
    <blockquote class="endorse-quote">“I have known Shayan since 2024 and have worked with him on NIAG’s perfusion MRI toolkit. As a computer engineering student, he showed exceptional eagerness to master medical imaging with a strong focus on perfusion MRI and became productive very quickly. He is organized and meticulous, with sharp attention to detail. His reports are clear, thorough, and actionable. Shayan communicates effectively with clinicians, actively seeks feedback, and turns it into practical improvements. He brings strong image processing expertise, programming skills, and the ability to research imaging methods and adapt them to clinical applications. He applies this knowledge creatively to solve difficult cases while maintaining scientific rigor. He is always on time, consistent in his execution, and shows strong responsibility for his work. I recommend Shayan for roles in medical image computing and I am confident he will elevate any project or team he joins.”</blockquote>
  </article>

  <!-- Amin THIRD -->
  <article class="endorse-card">
    <div class="endorse-header">
      <div class="endorse-avatar">
        <img src="images/amin-azirani.jfif" alt="Portrait of Amin Azirani">
      </div>
      <div class="endorse-meta">
        <h3 class="endorse-name">Amin Azirani, Solutions Engineer</h3>
        <div class="endorse-affil">cplace • Collegiality UG</div>
        <div class="endorse-links">
          <a href="https://www.linkedin.com/in/amin-azirani/" target="_blank" rel="noopener" aria-label="LinkedIn, Amin Azirani" title="LinkedIn">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM.5 8h4V23h-4V8zm7.49 0h3.84v2.05h.06c.53-1 1.82-2.05 3.75-2.05 4.01 0 4.75 2.64 4.75 6.08V23h-4v-7.02c0-1.68-.03-3.85-2.35-3.85-2.35 0-2.71 1.84-2.71 3.73V23h-4V8z"/></svg>
          </a>
          <a href="https://aminazirani.com/" target="_blank" rel="noopener" aria-label="Website, Amin Azirani" title="Website">
            <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 2a10 10 0 100 20 10 10 0 000-20zm7.94 9h-3.11a15.9 15.9 0 00-1.3-5 8.01 8.01 0 014.41 5zM12 4c1.12 0 2.77 2.24 3.4 6H8.6C9.23 6.24 10.88 4 12 4zM6.47 6a15.9 15.9 0 00-1.3 5H2.06A8.01 8.01 0 016.47 6zM2.06 13h3.11c.16 1.77.64 3.5 1.3 5a8.01 8.01 0 01-4.41-5zm5.14 0h6.6c-.63 3.76-2.28 6-3.3 6s-2.67-2.24-3.3-6zm6.93 5a15.9 15.9 0 001.3-5h3.11a8.01 8.01 0 01-4.41 5z"/></svg>
          </a>
        </div>
      </div>
    </div>
    <blockquote class="endorse-quote">“<em>Working with Shayan from 2022-2024 on our personalized guide creation app, I witnessed a software engineer who excelled at turning complex challenges into elegant solutions through creative problem-solving and systematic organization. His pre-AI era code showcased genuine innovation and craftsmanship, while his passionate advocacy for agile practices and thorough code reviews elevated our entire team's performance. Shayan's rare combination of technical creativity, structured execution, and unwavering reliability made him the engineer we trusted with our most critical features—any team would be fortunate to have him</em>.”</blockquote>
  </article>
</section>

# Courses

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      CS224W: Machine Learning with Graphs
    </div>
    <div class="experience-role">Stanford Online, March 2025</div>
    <div class="experience-topics">Topic: Graph Neural Networks</div>
  </div>
  <div class="experience-logo">
    <img src="../images/stanford-online.jpg" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Perfusion MRI
    </div>
    <div class="experience-role">Tehran University of Medical Sciences, Dec 2024</div>
    <div class="experience-topics">Topic: A PhD-level course taught by Dr. Mohammadi on DSC, DCE, and ASL perfusion MRI techniques.</div>
  </div>
  <div class="experience-logo">
    <img src="../images/TUMS.jfif" alt="Tehran University of Medical Sciences" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      How Diffusion Models Work
    </div>
    <div class="experience-role">DeepLearning.AI, Dec 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/deeplearning-ai.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      A/B Testing in Python
    </div>
    <div class="experience-role">365 Data Science, Aug 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/365ds.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Extreme Gradient Boosting with XGBoost
    </div>
    <div class="experience-role">DataCamp, Aug 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/datacamp.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      MLOps Concepts
    </div>
    <div class="experience-role">DataCamp, Aug 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/datacamp.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      ML mini-courses
    </div>
    <div class="experience-role">Kaggle, Aug 2024</div>
    <div class="experience-topics">Topics: Pandas, Computer Vision, Time Series, Geospatial Analysis, Feature Engineering, Data Visualization, ...</div>
  </div>
  <div class="experience-logo">
    <img src="../images/kaggle.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Deep Learning Specialization (5 Courses)
    </div>
    <div class="experience-role">DeepLearning.AI, May 2024</div>
  </div>
  <div class="experience-logo">
    <img src="../images/deeplearning-ai.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Scrum Foundations Workshop
    </div>
    <div class="experience-role">Scrum Alliance, Dec 2023</div>
  </div>
  <div class="experience-logo">
    <img src="../images/scrum.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Machine Learning Specialization (3 Courses)
    </div>
    <div class="experience-role">DeepLearning.AI, Sep 2023</div>
  </div>
  <div class="experience-logo">
    <img src="../images/deeplearning-ai.jfif" alt="Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      Python for Data Science, AI & Development
    </div>
    <div class="experience-role">Coursera, Jul 2023</div>
  </div>
  <div class="experience-logo">
    <img src="../images/coursera.jfif" alt="Logo" />
  </div>
</div>




# Hobbies

The motto I live by is *"Carpe Diem"*, which means *"Seize the Day"*.  
I believe the most valuable asset we have is the present moment, which is why I consider myself adventurous in all aspects of life, from work to personal experiences. I almost never say no to new opportunities, experiences, or challenges.

In my free time, I love doing sports, going trekking in nature, and capturing photographs.  
Here are some of my works:

<div class="hobbies-gallery">
  <img src="images/shayan-kebriti-Z_2Jtr-MyHQ-unsplash.jpg" alt="Waterfall in nature">
  <img src="images/shayan-kebriti-NeBdYxcrksc-unsplash.jpg" alt="Street with night lights in the forest">
  <img src="images/shayan-kebriti-8sKHVHCnVcg-unsplash.jpg" alt="Valley view with mountains">

  <!-- Horizontal images side by side -->
  <div class="wide-row">
    <img src="images/shayan-kebriti-Fx6t9zEnRyo-unsplash.jpg" alt="Camping in the mountains">
    <img src="images/shayan-kebriti-Yg5d7P3KQFg-unsplash.jpg" alt="Lake and forest landscape">
  </div>
</div>

<p style="margin-top:20px;">
  In case you’re curious, you can explore more of my adventures and photography on 
  <a href="https://unsplash.com/@i4mshayan" target="_blank">Unsplash</a>.
</p>





<!-- <script type="text/javascript" id="mmvst_globe" src="//mapmyvisitors.com/globe.js?d=HVZ1dytXl71ZnJux6Lqi9u_XgGZap1uRgqVjt2_TcTc"></script> -->

<br>
<br>
<br>
<br>