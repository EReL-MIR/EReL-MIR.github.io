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
h1 {
            color: #00008b; /* 深蓝色 */
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

<h1> Multimodal Document Retrieval Challenge Track</h1>

</div>


## Introduction

Currently, the majority of retrieval-augmented generation (RAG) models are designed to retrieve relevant text documents based on user queries. However, in real-world scenarios, users often need to retrieve multimodal documents, including text, images, tables, and charts. This requires a more sophisticated retrieval system that can handle multimodal information and provide relevant documents or passages based on user queries. Retrieving multimodal documents will help AI chatbots, search engines, and other applications provide more accurate and relevant information to users. 

The **Multimodal Document Retrieval Task** focuses on modeling passages from multimodal documents or web pages, leveraging textual and multimodal information for embedding modeling. The ultimate goal is to retrieve the relevant multimodal document or passage based on the user's text or multimodal query. 

---
## Participating
Please go to the challenge portal: [https://www.kaggle.com/competitions/multimodal-document-retrieval-challenge](https://www.kaggle.com/competitions/multimodal-document-retrieval-challenge)

## Tasks

### Task 1: MMDocIR – Multi-Modal Retrieval for Long Documents
This task is designed to evaluate the ability of retrieval systems to identify visually-rich information within documents. MMDocIR evaluation set includes 313 long documents averaging 65.1 pages, categorized into diverse domains: research reports, administration, industry, tutorials, workshops, academic papers, brochures, financial reports, guidebooks, government documents, laws, and news articles. Different domains feature distinct distributions of multi-modal information. 

**Sub-tasks**

- **Text → Multimodal Document Page Retrieval:** identify the most relevant pages within a document in response to a user query. The retrieval scope for each query is restricted to all pages in the given document.
  - **Datasets**: MMDocIR


---

In this challenge, MMDocIR evaluation set will be used for evaluation. 

Reference: https://huggingface.co/MMDocIR

---

### Task 2: M2KR – Open-Domain Vision Retrieval Benchmark
This task evaluates the ability of retrieval systems to retrieve visually-rich information in open-domain scenarios, including Wikipedia web pages. It involves diverse topics, forms (graphics, tables, text), and languages. The original M2KR dataset only include the extracted text from the Wikipedia pages. We have extended the dataset to include the screenshots from the Wikipedia pages.

**Subtasks:**

- **Image → Wiki Document Retrieval:** 
  - **Datasets:** WIT, KVQA.
- **Image+Text → Wiki Document Retrieval:**
  - **Datasets:** OVEN, OKVQA, Infoseek, E-VQA.

---
In this challenge, privately reserved test subset will be used for evaluation. 

Reference: [PreFLMR and M2KR Project Page](https://preflmr.github.io/)

Challenge Dataset: [M2KR-Challenge](https://huggingface.co/datasets/Jingbiao/M2KR-Challenge)

## Evaluation

Participants need to use one unified model to perform retrieval on both Task1 and Task2. Participants' submissions will be evaluated on their ability to accurately retrieve relevant multimodal documents or passages based on user queries. 

### Metrics:
**Recall@k** Measures the proportion of relevant documents retrieved in the top-k results.
We will be measuring the average score of recall@1, recall@3, and recall@5 for each tasks. The final score will be based on the average of the two tasks.


### Submission
The private test set is released for each of the dataset. The participants must upload the retrieved top5 `passage_id` for each test sample.

---

## Participation

To participate in this challenge, researchers are required to:
1. Develop multimodal retrieval systems capable of embedding modeling for multimodal queies and documents.
2. Submit a single system's outputs for evaluation based on the datasets specified in each task.

This track aims to push forward the boundaries of multimodal document retrieval, encouraging innovation in embedding modeling and search efficiency. Join us to contribute to the next-generation advancements in this exciting space!

---

## Timeline
Task Submission Start: Jan. 27th, 2025

Code Submission Start: Mar. 7th, 2025 (Delayed to Mar.15th)

Final Submission End: Mar. 15th, 2025 (Delayed to Mar.22nd)

Awarded Teams Release: Mar. 18th, 2025 (Delayed to Mar.25th)

---


## Awards

- **Overall Ranking** based on average recall scores across two tasks:
   - 1st Place: 1500 USD
   - 2nd Place: 1000 USD
   - 3rd Place: 500 USD
- **Multimodal Data Contribution Award**: 
  - Outstanding Team: 500 USD
- **Benchmark Contribution Award**: 
  - Outstanding Team: 500 USD
- **Travel Grant**: 
  - One team will be selected by the Challenge Chairs to receive a Travel Grant of 1000 USD.
  - The rewarded team need to given oral presentation on the workshop.

<strong>Note that all Awards are pre-tax amounts and include applicable taxes.</strong>

---

## Terms & Conditions
- Participants must submit their code to ensure reproducibility, which is essential for fair evaluation.
- For the Multimodal Data Contribution Award, teams must provide training data and highlight the novel contributions of their dataset.
- For the Benchmark Contribution Award, teams must submit a detailed technical report that includes extensive comparisons of methods and experimental code for each method.
- The Data/Benchmark Contribution Awards may be granted to the top three teams overall, and awards are not mutually exclusive.
- Each team can submit 3 solutions every day.


## Open Source License Requirement
The final winning teams must open-source their code under either the <strong>MIT License</strong> or the <strong>Apache License 2.0</strong>.


---

## References
1. Dong, K., Chang, Y., Deik Goh, X., Li, D., Tang, R., and Liu, Y. MMDocIR: Benchmarking Multi-Modal Retrieval for Long Documents (arXiv:2501.08828). arXiv. https://doi.org/10.48550/arXiv.2501.08828
2. Lin, W., Chen, J., Mei, J., Coca, A., & Byrne, B. (2023). Fine-grained Late-interaction Multi-modal Retrieval for Retrieval Augmented Visual Question Answering. Advances in Neural Information Processing Systems, 36, 22820–22840. 
3. Lin, W., Mei, J., Chen, J., & Byrne, B. (2024). PreFLMR: Scaling Up Fine-Grained Late-Interaction Multi-modal Retrievers. In L.-W. Ku, A. Martins, & V. Srikumar (Eds.), Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers) (pp. 5294–5316). Association for Computational Linguistics. https://doi.org/10.18653/v1/2024.acl-long.289



