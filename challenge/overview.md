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

## Motivation


In recent years, the rapid advancement of multimodal large models and the increasing demand for sophisticated information retrieval systems have highlighted the importance of integrating diverse modalities into real-world applications. Multimodal Information Retrieval (MIR) aims to address challenges where textual, visual, and other content modalities coexist, pushing the boundaries of search, recommendation, and information processing capabilities. 

To address these challenges, we have organized two major themes, each consisting of two tracks:

1. **Multimodal Document Retrieval Challenge Track**:
   - **ViDoRe**: Vision Document Retrieval Benchmark.
   - **M2KR**: Open-Domain Vision Retrieval Benchmark.

2. **MM-CTR Challenge Track**:
   - **Multimodal Item Embedding**.
   - **Multimodal CTR Prediction**.

These themes aim to foster innovation in:
- Developing retrieval systems capable of handling diverse multimodal data.
- Exploring efficient representation learning methods tailored for multimodal content.
- Encouraging solutions that bridge academic research and industrial practices in multimodal retrieval and recommendation.


---

## <a name='Organizers' style="color: inherit; text-decoration: none;"> Organizers </a>

<div class="organizers-container">
  <!-- 第一行 (5 人) -->
    <div class="organizer">
    <a href="https://xurige1995.github.io/" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/gexuri2.png" alt="Xuri Ge">
      <p><b>Xuri Ge</b><br>Shandong University</p>
    </a>
  </div>



  <div class="organizer">
    <a href="https://junchen-fu.github.io/" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/junchen-fu.jpg" alt="Junchen Fu">
      <p><b>Junchen Fu</b><br>University of Glasgow</p>
    </a>
  </div>
  

  
  <div class="organizer">
    <a href="https://jingbiao.me/about/?lang=en" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/jingbiao.jpg" alt="Jingbiao Mei">
      <p><b>Jingbiao Mei</b><br>University of Cambridge</p>
    </a>
  </div>
  
  <div class="organizer">
    <a href="https://fajieyuan.github.io/" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/fajie.jpg" alt="Fajie Yuan">
      <p><b>Fajie Yuan</b><br>Westlake University</p>
    </a>
  </div>
  
  <div class="organizer">
    <a href="http://jiemingzhu.github.io/" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/jmzhu.jpg" alt="Jieming Zhu">
      <p><b>Jieming Zhu</b><br>Huawei Noah's Ark Lab</p>
    </a>
  </div>

  <!-- 第二行 (3 人) -->
  <div class="organizer">
    <a href="" target="_blank">
      <img src="" alt="Jiabing Yan">
      <p><b>Jiabing Yan</b><br>Huawei</p>
    </a>
  </div>
  
  <div class="organizer">
    <a href="https://scholar.google.com/citations?user=OFiUwwEAAAAJ&hl=en" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/kuicai.jpg" alt="Kuicai Dong">
      <p><b>Kuicai Dong</b><br>Huawei Noah's Ark Lab</p>
    </a>
  </div>
  
  <div class="organizer">
    <a href="https://scholar.google.com/citations?user=YYnrPzEAAAAJ&hl=zh-CN&oi=ao" target="_blank">
      <img src="{{ site.baseurl }}/img/organizers/zhaocheng.jpg" alt="Zhaocheng Du">
      <p><b>Zhaocheng Du</b><br>Huawei Noah's Ark Lab</p>
    </a>
  </div>
</div>

<style>
.organizers-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-top:40px;
  justify-content: start;
}

.organizer {
  flex: 1 1 calc(25% - 20px);
  max-width: calc(25% - 20px);
  text-align: center;
  box-sizing: border-box;
}

.organizer img {
  width: 100%;
  max-width: 150px; /* 限制头像最大宽度为150px */
  height: auto;
  border-radius: 50%;
  display: block;
  margin: 0 auto; /* 居中显示 */
}

.organizer a {
  text-decoration: none;
  color: inherit;
}

.organizer p {
  margin-top: 10px;
}

/* 在大屏幕上，每行显示4个头像 */
@media (min-width: 1025px) {
  .organizer {
    flex: 1 1 calc(25% - 20px);
    max-width: calc(25% - 20px);
  }
}

/* 中等屏幕，每行显示3个头像 */
@media (max-width: 1024px) {
  .organizer {
    flex: 1 1 calc(33.33% - 20px);
    max-width: calc(33.33% - 20px);
  }
}

/* 小屏幕，每行显示2个头像 */
@media (max-width: 768px) {
  .organizer {
    flex: 1 1 calc(50% - 20px);
    max-width: calc(50% - 20px);
  }
}

/* 超小屏幕，每行显示1个头像，并缩小头像尺寸 */
@media (max-width: 480px) {
  .organizer {
    flex: 1 1 calc(100% - 20px);
    max-width: calc(100% - 20px);
  }
  
  .organizer img {
    max-width: 80px; /* 在超小屏幕上，将头像最大宽度限制为80px */
  }
}

</style>


## <a name='Organization' style="color: inherit; text-decoration: none;"> Sponsored by Huawei</a>


<style>
.organization-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 50px;
  margin-bottom: 50px;
  justify-content: center; /* 将子元素居中对齐 */
}

.organization {
  flex: 1 1 calc(25% - 20px);
  max-width: calc(25% - 20px);
  text-align: center;
  box-sizing: border-box;
}

.organization img {
  width: 100%;
  max-width: 150px; /* 限制头像最大宽度为150px */
  height: auto;
  display: block;
  margin: 0 auto; /* 图片自身居中 */
}

.organization a {
  text-decoration: none;
  color: inherit;
}

.organization p {
  margin-top: 10px;
}

/* 在大屏幕上，每行显示4个头像 */
@media (min-width: 1025px) {
  .organization {
    flex: 1 1 calc(33% - 20px);
    max-width: calc(33% - 20px);
  }
}

/* 中等屏幕，每行显示3个头像 */
@media (max-width: 1024px) {
  .organization {
    flex: 1 1 calc(33.33% - 20px);
    max-width: calc(33.33% - 20px);
  }
}

/* 小屏幕，每行显示2个头像 */
@media (max-width: 768px) {
  .organization {
    flex: 1 1 calc(50% - 20px);
    max-width: calc(50% - 20px);
  }
}

/* 超小屏幕，每行显示1个头像，并缩小头像尺寸 */
@media (max-width: 480px) {
  .organization {
    flex: 1 1 calc(100% - 20px);
    max-width: calc(100% - 20px);
  }
  
  .organization img {
    max-width: 80px; /* 在超小屏幕上，将头像最大宽度限制为80px */
  }
}
</style>