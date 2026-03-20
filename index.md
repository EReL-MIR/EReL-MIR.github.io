---
layout: page
description: ""
---
<h1 style="text-align: center; font-size: 28px; color: inherit; line-height: 1.5;">
    <span style="display: inline-flex; align-items: center; white-space: nowrap;">
        <img src="/img/erelmire.jpg" alt="EReL Logo"
             style="width: 60px; height: 60px; border-radius: 50%; margin-top:-20px; margin-right: 5px; position: relative; top: 15px;">
    </span>
    The 2<sup>nd</sup> EReL@MIR Workshop on Efficient Representation Learning for <br> Multimodal Information Retrieval
</h1>

The 2nd EReL@MIR Workshop will be co-located with **ACM Multimedia 2026** in Rio de Janeiro, Brazil (10–14 November 2026).

Multimodal information retrieval (MIR) underpins modern multimedia services across both industry and academia — from large-scale recommendation and e-commerce search to general-purpose web and conversational search systems. The rapid progress of large pre-trained foundation models for language and vision–language learning (e.g., Qwen, LLaVA, and CLIP) has significantly reshaped how multimodal representations are learned and transferred across tasks. These advances have enabled strong performance in MIR settings such as web search, cross-modal retrieval, and multimodal recommender systems.

Despite these gains, deploying large multimodal models in real-world MIR pipelines exposes a persistent gap between effectiveness and system feasibility. Production MIR systems must satisfy strict latency and throughput targets while controlling VRAM, storage, and end-to-end serving costs, yet efficiency is still under-reported and inconsistently evaluated in much of the literature. This limits fair comparison, reproducibility, and practical adoption at scale — motivating research on efficient adaptation, fusion, compression, indexing, and scalable serving for MIR.

Two emerging shifts have further expanded the MIR design space and sharpened the urgency of efficiency research. First, **omni-modal models** unify a broader set of modalities (text, image, audio, video) within a single framework, enabling richer interactions but exacerbating computational and serving constraints: their larger scale and prompt-dependent representations make embedding pre-computation and caching difficult. Second, **generative MIR** approaches that generate identifiers or structured candidates introduce new efficiency and reliability challenges, including decoding-time latency, output validity and controllability, and tokenization complexity.

We therefore propose the 2nd EReL@MIR workshop at ACM Multimedia 2026 as a timely venue to advance efficiency-aware multimodal representation learning and multimedia retrieval. The workshop complements the main MM 2026 program by strengthening core multimedia themes — including multimodal learning, vision–language modeling, multimedia retrieval, recommendation, and multimodal generation — through the lens of efficiency, deployability, and cost-aware system design. The workshop has four main goals: (i) promote research on efficiency-aware multimodal learning for large-scale multimedia applications; (ii) encourage unified metrics and benchmarks that jointly evaluate effectiveness and system cost; (iii) advance deployable solutions for real-world multimedia retrieval and generation systems; and (iv) stimulate discussion on emerging omni-modal and generative paradigms under realistic computational constraints.

Previous edition (2025) archive: [https://erel-mir.github.io/2025/](https://erel-mir.github.io/2025/)

Conference homepage: [https://2026.acmmm.org/index.html](https://2026.acmmm.org/index.html)

## <a name='Call for Papers' style="color: inherit; text-decoration: none;text-align: center;"> Call for Papers </a>
We invite researchers to submit their latest work on efficient multimodal representation learning for multimodal information retrieval (MIR). Topics include, but are not limited to:

- Efficient Multimodal Representation Adaptation based on Multimodal Foundation Models
- Data-Efficiency in Multimodal Representation Learning
- Efficient Multimodal Fusion for Representation Learning
- Efficient Cross-Modality Interaction for MIR
- Real-Time Inference for Multimodal Representations
- Efficient MIR Foundation Models
- Benchmarks and Metrics for Multimodal Representation Learning Efficiency
- Efficient Omni-modal MIR
- Efficient Multimodal Generative MIR

## Submission Guidelines
Submissions of papers must be at least 4 pages and at most 8 pages (including figures, tables, proofs, appendixes, acknowledgments, and any content except references) in length, with unlimited pages for references. Submissions must be in English and in PDF format, using the ACM two-column conference format. Suitable templates are available from the [ACM Website](https://www.acm.org/publications/proceedings-template) (use the "sigconf" proceedings template for LaTeX and the Interim Template for Word).

The review process will be done with our program committee. Selection depends on technical soundness and relevance to the workshop community. At least one author of each accepted paper must attend the workshop on-site and present their work.

## <a name='Important Dates' style="color: inherit; text-decoration: none; text-align: center;"> Important Dates </a>
- Contribution Submission: **16-July**
- Author Notification: **06-August**
- Camera-Ready: **20-August**
- Author Registration: **20-August**

## <a name='Organizers' style="color: inherit; text-decoration: none;"> Organizers </a>

<div class="organizer-grid">
  <div class="organizer-card">
    <a href="https://junchen-fu.github.io/" target="_blank">
      <img src="/img/organizers/junchen-fu.jpg" alt="Junchen Fu">
      <p><b>Junchen Fu</b><br>University of Glasgow</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://xurige1995.github.io/" target="_blank">
      <img src="/img/organizers/gexuri2.png" alt="Xuri Ge">
      <p><b>Xuri Ge</b><br>Shandong University</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://xinxin-me.github.io/" target="_blank">
      <img src="/img/organizers/xinxin.png" alt="Xin Xin">
      <p><b>Xin Xin</b><br>Shandong University</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://alexiskz.wordpress.com/" target="_blank">
      <img src="/img/organizers/alex.png" alt="Alexandros Karatzoglou">
      <p><b>Alexandros Karatzoglou</b><br>Amazon</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://iarapakis.github.io/" target="_blank">
      <img src="/img/organizers/ioannis2.png" alt="Ioannis Arapakis">
      <p><b>Ioannis Arapakis</b><br>Telefónica Scientific Research</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://www.xiwangeric.com/" target="_blank">
      <img src="/img/organizers/xi-wang.jpg" alt="Xi Wang">
      <p><b>Xi Wang</b><br>University of Sheffield</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://liu.qijiong.work/" target="_blank">
      <img src="/img/organizers/qijiong-liu.jpg" alt="Qijiong Liu">
      <p><b>Qijiong Liu</b><br>The Hong Kong Polytechnic University</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://liqian-bio.github.io/" target="_blank">
      <img src="/img/organizers/qian-li.jpg" alt="Qian Li">
      <p><b>Qian Li</b><br>Beijing University of Posts and Telecommunications</p>
    </a>
  </div>
  <div class="organizer-card">
    <a href="https://www.dcs.gla.ac.uk/~jj/" target="_blank">
      <img src="/img/organizers/joemon.png" alt="Joemon M. Jose">
      <p><b>Joemon M. Jose</b><br>University of Glasgow</p>
    </a>
  </div>
</div>

<style>
.organizer-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 24px;
}

.organizer-card {
  flex: 1 1 220px;
  max-width: 260px;
  text-align: center;
}

.organizer-card img {
  width: 140px;
  height: 140px;
  object-fit: cover;
  border-radius: 50%;
  transition: opacity 0.2s;
}

.organizer-card a {
  text-decoration: none;
  color: inherit;
}

.organizer-card a:hover img {
  opacity: 0.8;
}

.organizer-card a:hover p {
  text-decoration: underline;
}
</style>

## <a name='Program Committee' style="color: inherit; text-decoration: none;"> Program Committee</a>
- **Jiayi Ji**, National University of Singapore
- **Mingyue Cheng**, University of Science and Technology of China
- **Ying Zhou**, Shandong University
- **Hengchang Hu**, National University of Singapore
- **Yumeng Wang**, Leiden University
- **Fuhai Chen**, Fuzhou University
- **Hui Li**, Xiamen University
- **Songpei Xu**, University of Glasgow
- **Zheng Yuan**, The Hong Kong Polytechnic University
- **Jiaqi Zhang**, University of Queensland

## <a name='Contact' style="color: inherit; text-decoration: none;"> Contact</a>
If you have any questions about EReL@MIR, contact:

- <a href="mailto:j.fu.3@research.gla.ac.uk">j.fu.3@research.gla.ac.uk</a>
- <a href="mailto:xuri.ge@sdu.edu.cn">xuri.ge@sdu.edu.cn</a>
- <a href="mailto:joemon.jose@glasgow.ac.uk">joemon.jose@glasgow.ac.uk</a>

