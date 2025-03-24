---
layout: page
title: MIR Challenge
header-img: none
---
<style>
  .intro-header {
    display: none;
}

/* 导航栏样式 */
.navbar {
    display: flex;
    justify-content: center;
    background-color: rgb(27, 32, 122);
    color: rgb(255, 255, 255);
    padding: 10px 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
    margin-bottom: 2px;
    flex-wrap: wrap;
}

.navbar a {
    margin: 0 20px;
    text-decoration: none;
    color: rgb(255, 255, 255);
    font-weight: bold;
    transition: color 0.3s, border-bottom 0.3s;
}

.navbar a:hover {
    color: #007acc;
    border-bottom: 2px solid #007acc;
}

@media screen and (max-width: 768px) {
    .navbar {
        justify-content: space-around;
        padding: 10px;
    }

    .navbar a {
        margin: 5px;
        font-size: 14px;
    }
}

/* 内容区域样式 */
.tab-content {
    padding: 20px;
    animation: fade-in 0.5s ease;
}

/* 动画效果 */
@keyframes fade-in {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
    }
.image-container {
    width: 70%; /* 图片容器宽度 */
    margin: 0px auto; /* 居中 */
    text-align: center; /* 文本居中 */
    background-color:rgb(255, 255, 255); /* 背景颜色（可选） */
    padding: 0px; /* 容器内边距 */
    border-radius: 8px; /* 圆角边框 */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* 轻微阴影效果 */
}

/* 图片样式 */
.image-container img {
    width: 100%; /* 图片宽度 */
    height: auto; /* 等比例缩放 */
    border-radius: 4px; /* 图片圆角（可选） */
}

</style>

<div class="navbar">
    <a href="{{ site.baseurl }}/challenge/overview/">Overview</a>
    <a href="{{ site.baseurl }}/challenge/mdr-track1/">Track 1</a>
    <a href="{{ site.baseurl }}/challenge/mmctr-track2/">Track 2</a>
    <a href="{{ site.baseurl }}/challenge/results/">Results</a>
    <a href="{{ site.baseurl }}/challenge/discussion/">Discussion</a>
    <a href="{{ site.baseurl }}/">Return to Workshop Home</a>
</div>

<div class="image-container">
    <img src="{{ site.baseurl }}/img/challenge.png" alt="Challenge Image">
</div>


<div style="text-align: center;">
  <h1>Track 1 Winners-Multimodal Document Retrieval Challenge Track</h1>
  <h2>TBA</h2>
  <br>
  <h1>Track 2 Winners-Multimodal CTR Prediction Challenge Track</h1>
  <table border="1" cellspacing="0" cellpadding="10" style="margin: 0 auto; border-collapse: collapse;">
    <tr style="background-color: #a8d08d;">
      <th>Rank/Award</th>
      <th>Team Name</th>
      <th>Code Link</th>
    </tr>
    <tr>
      <td>1st Place</td>
      <td>momo</td>
      <td>https://github.com/pinskyrobin/WWW2025_MMCTR</td>
    </tr>
    <tr>
      <td>2nd Place</td>
      <td>DISCO.AHU</td>
      <td>https://github.com/salmon1802/QIN</td>
    </tr>
    <tr>
      <td>3rd Place</td>
      <td>jzzx.NTU</td>
      <td></td>
    </tr>
    <tr>
      <td>Task 1 Winner</td>
      <td>delorean</td>
      <td></td>
    </tr>
    <tr>
      <td>Task 2 Winner</td>
      <td>zhou123</td>
      <td>https://github.com/Lattice-zjj/MMCTR_Code</td>
    </tr>
  </table>
</div>
<h2>Upon receiving the open-source code from the winning teams, as demonstrated above, it will be made publicly available for a three-day review period. During this time, anyone who identifies potential misconduct—such as plagiarism or other unethical behavior—is encouraged to report it to the organizers via <a href="mailto:erelmir.workshop@gmail.com">erelmir.workshop@gmail.com</a>. Submissions that pass this public review will be officially confirmed as the final winners.</h2>
