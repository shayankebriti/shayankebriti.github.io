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


</style>

<!-- {% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %} -->

<span class='anchor' id='about-me'></span>


# About Me



# Publications
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Submitted</div>
      <img src='images/fractmorph.png' alt="sym" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

  <strong>FractMorph: A Fractional Fourier-Based Multi-Domain Transformer for Deformable Image Registration</strong>

  <!-- Author list with Scholar icons -->
  <p>
    <strong>Shayan Kebriti</strong><sup>1</sup>,
    Shahabedin Nabavi<sup>1</sup>
    <a href="https://scholar.google.com/citations?user=D_mPA6sAAAAJ&hl" target="_blank">
      <img src="https://upload.wikimedia.org/wikipedia/commons/c/c7/Google_Scholar_logo.svg"
           alt="Google Scholar" width="16" style="vertical-align: middle; margin-left: 4px;">
    </a>,
    Ali Gooya<sup>2,3</sup>
    <a href="https://scholar.google.com/citations?user=H7w9icgAAAAJ&hl" target="_blank">
      <img src="https://upload.wikimedia.org/wikipedia/commons/c/c7/Google_Scholar_logo.svg"
           alt="Google Scholar" width="16" style="vertical-align: middle; margin-left: 4px;">
    </a>
  </p>

  [[arXiv](https://arxiv.org/abs/2508.12445)]
  [[Paper](https://arxiv.org/pdf/2508.12445)]
  [[Github](https://github.com/shayankebriti/FractMorph)]

  FractMorph is a novel 3D dual-parallel transformer for deformable image registration. Its Fractional Cross-Attention blends multi-scale spectral–spatial features via fractional Fourier transforms, achieving state-of-the-art results on <strong>intra-patient cardiac</strong> and <strong>atlas-to-patient cerebral</strong> MRI benchmarks.
  
  <!-- Affiliations -->
  <p style="margin-top: 4px;">
    <sup>1</sup> Faculty of Computer Science and Engineering, Shahid Beheshti University, Tehran, Iran<br>
    <sup>2</sup> School of Computing Science, University of Glasgow, Glasgow, UK<br>
    <sup>3</sup> Alan Turing Institute, London, UK
  </p>
  </div>
</div>


# Education

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>Sep 2021 - Now</strong><br/>
      Bachelor, Computer Engineering, Shahid Beheshti Univeristy, Tehran, Iran
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/Sbu-logo.png" alt="SBU logo" />
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
    <div class="experience-role">ML Engineer & Data Scientist</div>
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
    <div class="experience-role">AI Research Intern</div>
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