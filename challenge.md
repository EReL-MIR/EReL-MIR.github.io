---
layout: page
title: MIR Challenge
---

<h1 style="text-align: center; font-size: 28px; color: inherit; line-height: 1.5;">
    Multimodal Information Retrieval Challenge for The 1<sup>st</sup> EReL@MIR Workshop
</h1>

## <a name='EReL@MIR Track'> Multimodal Document Retrieval Track </a>

### Introduction

Currently, the majority of retrieval-augmented generation (RAG) models are designed to retrieve relevant text documents based on user queries. However, in real-world scenarios, users often need to retrieve multimodal documents, including text, images, tables, and charts. This requires a more sophisticated retrieval system that can handle multimodal information and provide relevant documents or passages based on user queries. Retrieving multimodal documents will help AI chatbots, search engines, and other applications provide more accurate and relevant information to users.

The **Multimodal Document Retrieval Task** focuses on modeling passages from multimodal documents or web pages, leveraging textual and multimodal information for embedding modeling. The ultimate goal is to retrieve the relevant multimodal document or passage based on the user's text or multimodal query.

### Tasks

#### Task 1: ViDoRe – Vision Document Retrieval Benchmark
This task is designed to evaluate the ability of retrieval systems to identify visually-rich information within documents. It covers multiple topics, forms (graphics, tables, text), and languages, providing a robust benchmark for retrieval scenarios.

**Datasets Include:**
- **DocVQA**: Industrial documents.
- **InfoVQA**: Infographics.
- **TAT-DQA**: Financial report tables.
- **arXiVQA**: Academic charts.
- **TabFQuAD**: Tables.

**Application Scenarios:** Industry reports from sectors such as energy, government/administration, healthcare, artificial intelligence, and environmental studies.

#### Task 2: M2KR – Open-Domain Vision Retrieval Benchmark
This task evaluates the ability of retrieval systems to retrieve visually-rich information in open-domain scenarios, including Wikipedia web pages. It involves diverse topics, forms (graphics, tables, text), and languages. The dataset includes screenshots from Wikipedia pages and extracted text.

### Evaluation and Metrics

**Metrics:**
- **Recall@k:** Measures the proportion of relevant documents retrieved in the top-k results. Average scores of recall@1, recall@5, and recall@10 will be computed.

---

## <a name='WWW Challenge'> MM-CTR Challenge </a>

### Introduction

With the development of multimodal large models and the popularity of content recommendation applications, multimodal recommendation has become one of the most prominent paradigms in the research community. To promote breakthroughs in this field, we organize a Multimodal CTR prediction (MM-CTR) Challenge at the WWW 2025 EReL@MIR workshop. The challenge consists of two sub-tasks:

1. **Multimodal Item Embedding**: Developing multimodal representation learning and fusion methods tailored for recommendation tasks.
2. **Multimodal CTR Prediction**: Designing CTR prediction models that effectively utilize multimodal representations to enhance recommendation performance.

### Dataset Description

We use the MicroLens dataset (specifically the MicroLens-1M version) released by Westlake University for the MM-CTR Challenge. This dataset contains 1M users and 9.1M user-item interaction records, with detailed item content features (e.g., titles, covers). Public data is provided for training, and private data for evaluation.

### Tasks

#### Task 1: Multimodal Item Embedding
Participants must design algorithms to extract multimodal embeddings for recommendation tasks. Extracted embeddings should be saved in a specified format and combined with ID features for downstream CTR model evaluation.

#### Task 2: Multimodal CTR Prediction
Participants will optimize the CTR model using embeddings provided by organizers. The designed CTR model must be trained in an end-to-end manner.

### Evaluation and Rules

**Metrics:** AUC will be used to evaluate performance. Submissions are ranked based on reproducible results from provided code.

---

## <a name='Organization' style="color: inherit; text-decoration: none;"> Sponsored by </a>
  <div class="organization">
    <a href="https://gair-lab.github.io/" target="_blank">
      <img src="../img/organization/huawei-logo.png" alt="HUAWEI">
    </a>
  </div>

  <a href="../">Link To Back</a>
  
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