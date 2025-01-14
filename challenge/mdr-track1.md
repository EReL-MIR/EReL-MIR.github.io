---
layout: page
title: MIR Challenge Track1
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
    padding: 5px 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
    margin-bottom: 10px;
}

.navbar a {
    margin: 0 15px;
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

## Introduction

Currently, the majority of retrieval-augmented generation (RAG) models are designed to retrieve relevant text documents based on user queries. However, in real-world scenarios, users often need to retrieve multimodal documents, including text, images, tables, and charts. This requires a more sophisticated retrieval system that can handle multimodal information and provide relevant documents or passages based on user queries. Retrieving multimodal documents will help AI chatbots, search engines, and other applications provide more accurate and relevant information to users. 

The **Multimodal Document Retrieval Task** focuses on modeling passages from multimodal documents or web pages, leveraging textual and multimodal information for embedding modeling. The ultimate goal is to retrieve the relevant multimodal document or passage based on the user's text or multimodal query. 

---

## Tasks

### Task 1: MMDocIR – Multi-Modal Retrieval for Long Documents

This task is designed to evaluate the ability of retrieval systems to identify visually-rich information within documents. MMDocIR evaluation set includes 313 long documents averaging 65.1 pages, categorized into diverse domains: research reports, administration, industry, tutorials, workshops, academic papers, brochures, financial reports, guidebooks, government documents, laws, and news articles. Different domains feature distinct distributions of multi-modal information. 

**Sub-tasks**

- **Page-level Retrieval**: identify the most relevant pages within a document in response to a user query.
- **Layout-level Retrieval**:  retrieve most relevant layouts. The layouts are defined as the fine-grained elements such as paragraphs, equations, figures, tables, and charts. This task allows for a more nuanced content retrieval, honing in on specific information that directly answers user queries.

---

In this challenge, MMDocIR evaluation set (which is yet to publish) will be used for evaluation. 

Reference: https://huggingface.co/MMDocIR

---

### Task 2: M2KR – Open-Domain Vision Retrieval Benchmark

This task evaluates the ability of retrieval systems to retrieve visually-rich information in open-domain scenarios, including Wikipedia web pages. It involves diverse topics, forms (graphics, tables, text), and languages. The original M2KR dataset only include the extracted text from the Wikipedia pages. We have extended the dataset to include the screenshots from the Wikipedia pages.

**Subtasks:**

- **Image → Wiki Document Search:** 
  - **Datasets:** WIT, KVQA.
- **Image+Text → Wiki Document Search:**
  - **Datasets:** OVEN, OKVQA, Infoseek, E-VQA.

---

In this challenge, privately reserved test subset will be used for evaluation. 

Reference: https://preflmr.github.io/

## Evaluation

Participants' submissions will be evaluated on their ability to accurately retrieve relevant multimodal documents or passages based on user queries. 

### Metrics:

**Recall@k** Measures the proportion of relevant documents retrieved in the top-k results.
We will be measuring the average score of recall@1, recall@5, and recall@10 for each tasks.

### Ranking

We will rank the participants by the average of the two tasks's recall scores. 

### Submition

The private test set is released for each of the dataset. The participants will be required to upload the retrieved top10 `passage_id` for each test sample to Kaggle. The platform will automatically compute the score. 

---

## Participation

To participate in this challenge, researchers are required to:

1. Develop multimodal retrieval systems capable of embedding modeling for multimodal queies and documents.
2. Submit a single system's outputs for evaluation based on the datasets specified in each task.

This track aims to push forward the boundaries of multimodal document retrieval, encouraging innovation in embedding modeling and search efficiency. Join us to contribute to the next-generation advancements in this exciting space!

---

## References

1. to be updated with arxiv paper link
2. Lin, W., Mei, J., Chen, J., & Byrne, B. (2024). PreFLMR: Scaling Up Fine-Grained Late-Interaction Multi-modal Retrievers (arXiv:2402.08327). arXiv. https://doi.org/10.48550/arXiv.2402.08327
3. Lin, W., Chen, J., Mei, J., Coca, A., & Byrne, B. (2023). Fine-grained Late-interaction Multi-modal Retrieval for Retrieval Augmented Visual Question Answering (arXiv:2309.17133; Version 2). arXiv. https://doi.org/10.48550/arXiv.2309.17133

