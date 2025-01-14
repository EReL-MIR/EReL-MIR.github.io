---
layout: page
title: MIR Challenge
header-img: img/challenge.png
---
<style>
/* 容器样式 */
.intro-header {
    width: 70%;
    margin: 0 auto;
    padding: 0;
    background-color: white; /* 设置背景颜色为白色 */
}

/* 图片样式 */
.header-img {
    width: 100%;
    height: auto;
    display: block;
    margin: 0 auto;
}

/* 导航栏样式 */
.navbar {
    display: flex;
    justify-content: center;
    background-color: #f4f4f4;
    padding: 10px 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
    margin-bottom: 20px;
}

.navbar a {
    margin: 0 15px;
    text-decoration: none;
    color: #333;
    font-weight: bold;
    transition: color 0.3s, border-bottom 0.3s;
}

.navbar a:hover {
    color: #007acc;
    border-bottom: 2px solid #007acc;
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

</style>

<div class="navbar">
    <a href="{{ site.baseurl }}/challenge/overview/">Overview</a>
    <a href="{{ site.baseurl }}/challenge/mdr-track1/">Track 1</a>
    <a href="{{ site.baseurl }}/challenge/mmctr-track2/">Track 2</a>
    <a href="{{ site.baseurl }}/challenge/results/">Results</a>
    <a href="{{ site.baseurl }}/challenge/discussion/">Discussion</a>
    <a href="{{ site.baseurl }}">Back to Workshop</a>
</div>
