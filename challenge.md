---
layout: page
title: MIR Challenge
---

<h1 style="text-align: center; font-size: 28px; color: inherit; line-height: 1.5;">
    <span style="display: inline-flex; align-items: center; white-space: nowrap;">
        <img src="../img/erelmire.jpg" alt="EReL Logo"
             style="width: 60px; height: 60px; border-radius: 50%; margin-top:-20px; margin-right: 5px; position: relative; top: 15px;">
    </span>
    Multimodal Information Retrieval Challenge for The 1<sup>st</sup> EReL@MIR Workshop
</h1>

## <a name='Organization' style="color: inherit; text-decoration: none;"> Sponsored by </a>
  <div class="organization">
    <a href="https://gair-lab.github.io/" target="_blank">
      <img src="../img/organization/huaiwei-logo.png" alt="HUAWEI">
    </a>
  </div>

  <a href="../">Link To Back</a>
  
<style>
.organization-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 40px;
  margin-bottom: 40px;
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
  max-width: 250px; /* 限制头像最大宽度为150px */
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