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
    background-color:rgb(27, 32, 122);
    color:rgb(255,255,255);
    padding: 2px 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
    margin-bottom: 5px;
}

.navbar a {
    margin: 0 5px;
    text-decoration: none;
    color: rgb(255,255,255);
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
    <a href="{{ site.baseurl }}">Return to Workshop Home</a>
</div>

<div class="image-container">
    <img src="{{ site.baseurl }}/img/challenge.png" alt="Challenge Image">
</div>



## Motivation


In recent years, the rapid advancement of multimodal large models and the increasing demand for sophisticated information retrieval systems have highlighted the importance of integrating diverse modalities into real-world applications. Multimodal Information Retrieval (MIR) aims to address challenges where textual, visual, and other content modalities coexist, pushing the boundaries of search, recommendation, and information processing capabilities. 

To address these challenges, we have organized two major themes, each consisting of two tracks:

1. **[Multimodal Document Retrieval Track](#multimodal-document-retrieval-track)**:
   - **ViDoRe**: Vision Document Retrieval Benchmark.
   - **M2KR**: Open-Domain Vision Retrieval Benchmark.

2. **[MM-CTR Challenge](#mm-ctr-challenge)**:
   - **Multimodal Item Embedding**.
   - **Multimodal CTR Prediction**.

These themes aim to foster innovation in:
- Developing retrieval systems capable of handling diverse multimodal data.
- Exploring efficient representation learning methods tailored for multimodal content.
- Encouraging solutions that bridge academic research and industrial practices in multimodal retrieval and recommendation.


---

## <a name='mm-ctr-challenge'> 2. MM-CTR Challenge </a>


With the development of multimodal large models and the popularity of content recommendation applications, multimodal recommendation has become one of the most prominent paradigms in the research community. To promote breakthroughs in this field, we organize a Multimodal CTR prediction (MM-CTR) Challenge at the WWW 2025 EReL@MIR workshop. To meet the low-latency requirements of online inference in industrial applications,  we have divided the MM-CTR Challenge into two sub-tasks: Multimodal Item Embedding and Multimodal CTR Prediction. The first task centers on developing multimodal representation learning and fusion methods tailored for recommendation tasks, while the second focuses on designing CTR prediction models that effectively utilize multimodal representations to enhance recommendation performance. Through in-depth exploration on these two tasks, we aim to broden the boundary of multimodal recommendation and providing solutions with practical value and insights for industrial recommendation systems.

### Dataset Description

We use the MicroLens dataset (specifically the MicroLens-1M version) released by Westlake University [1] for MM-CTR Challenge. This dataset contains 1M users and 9.1M user-item interaction records,  with detailed item content features (e.g., titles, covers). This challenge will use public data for training and private data for evaluation, respectively. Data details will be announced later.

### Task 1: Multimodal Item Embedding

This challenge aims to explore multimodal item embedding extraction methods that enhancing recommendation tasks. The organizers will provide downstream CTR model and evaluation datasets to validate the effectiveness of proposed methods. Participants are free to use open-source multimodal models, and design algorithms to extract multimodal embeddings. Extracted embeddings must be saved in a specified format and combined with ID features as input for downstream CTR model evaluation.

>  Task Input:

* User historical interaction data
* Item multimodal data (including attributes, title, cover)

> Task Output:

* Multimodal embedding features (dimension size: 128)

#### Evaluation

Participants are required to use the provided CTR model to evaluate the effectiveness of the multimodal embeddings. Specifically, they should replace the embedding features in the CTR model's input with the features extracted in Task 1, retrain the model, evaluate its performance on the validation set, and predict pCTR on the test set for submission. In the preliminary round, participants only need to submit the pCTR prediction results. In the final round, participants must also submit reproducible training and inference code for the multimodal embeddings. The final leaderboard will be ranked based on reproducible submission results. The evaluation metric is AUC.

#### Constrain

+ Using any data outside the provided dataset is not allowed.

+ If large models are used to extract embeddings, only open-source versions are allowed.

<a href="../">Back</a> 
<a href="./">Home</a>



### Task 2: Multimodal CTR Prediction

This challenge aims to explore what multimodal recommendation model can effectively leverage the multimodal embedding and achive better performance. The organizers will provide extracted multimodal embedding (from Task 1) and user interaction data splits. Participants can optimize and improve the multimodal recommendation model based on the provided baseline model to enhance the CTR prediction result. Finally, participants will submit the predicted pCTR on the test set for competition.

>  Task Input:

* User historical interaction data
* All items' multimodal embedding

> Task Output:

* Predicted pCTR for test set samples

### Evaluation

Participants are required to use the multimodal embeddings provided by organizers  to evaluate the performance of the CTR model. Specifically, they should replace the provided basedline model with the customized CTR model designed in Task 2, train the model, evaluate its performance on the validation set, and predict pCTR on the test set for submission. In the preliminary round, participants only need to submit the pCTR prediction results. In the final round, participants must also submit reproducible training and inference code for the multimodal embeddings. The final leaderboard will be ranked based on reproducible submission results. The evaluation metric is AUC.

### Constrain

+ Using pretrained large model is not allowed.
+ The designed CTR model must be trained in an end-to-end manner.

+ For practical application considerations, only neural network models are allowed; Ensemble methods are not allowed for training or testing.



### Submission Type

Participants can choose one submission types listed below to engage in the challenge. We encourage participants to take on both challenges (Task 1 & Task 2) to fully understand the end-to-end process of multimodal recommendation application and design better solutions, thereby earning more rewards.

**Task 1 only**: In this setting, the CTR model is fixed, and the focus is on optimizing the embeddings. Participants are not allowed to modify the model code used to evaluate the embeddings, but can adjust specified hyperparameters.

**Task 2 only**: In this setting, the embeddings are fixed, and the focus is on optimizing the CTR model. Participants are not allowed to change the input features, but can optimize the model structure and hyperparameters.

**Task 1 & 2**: In this setting, both the embeddings and the CTR model are optimized simultaneously. Participants can modify both the embeddings and the CTR model, but no additional features are allowed.

The challenge organizers will reproduce results based on the team's submitted code and reproducibility guidelines, and the results will be publicly announced on the official website.

### Timeline

Task Submission Start: Jan. 22nd, 2025

Code Submission Start: Mar. 

Final Submission End: 

### Awards

Participants are required to submit their source code for model reproduction and final award competation. The review panel will reproduce results based on the leaderboard rankings, from highest to lowest. The top three teams in the reproduced results will be awarded as the 1st, 2nd, and 3rd place teams. Additionally, an Embedding Winner and a Model Winner will be selected for Task-1 and Task-2, respectively. If results cannot be reproduced or a team wins multiple awards, the prize will be passed to the next team.

+ 1st Team: 1500 USD + Travel Grant of 1000 USD  
+ 2nd Team: 1000 USD
+ 3rd Team: 500 USD

### Rules

1. Awarded teams must comply with relevant open-source licenses and release their competition solutions.
2. Awarded teams are required to present their solutions either on-site at the workshop or online.



### Reference

[1] Yongxin Ni, Yu Cheng, Xiangyan Liu, Junchen Fu, Youhua Li, Xiangnan He, Yongfeng Zhang, Fajie Yuan, A Content-Driven Micro-Video Recommendation Dataset at Scale, Arxiv 2023.

<a href="../">Back</a> 
<a href="./">Home</a>


## <a name='Organization' style="color: inherit; text-decoration: none;"> Sponsored by </a>
  <div class="organization">
    <a href="https://gair-lab.github.io/" target="_blank">
      <img src="../img/organization/huawei-logo.png" alt="HUAWEI">
    </a>
  </div>


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