---
permalink: /
lang: en
title: "Shuang Sun"
excerpt: "M.S. student at Gaoling School of Artificial Intelligence (RUC). Research: NLP, LLMs, and Agents."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<!-- <div style="margin-top: 0.6rem; margin-bottom: 1.0rem;">
  <a href="#en">English</a> · <a href="#zh">中文</a>
</div> -->



<span class='anchor' id='en'></span>
<span class='anchor' id='about-me'></span>

## 👋 About Me

I am a first-year M.S. student at the [Gaoling School of Artificial Intelligence (GSAI)](http://ai.ruc.edu.cn/), [Renmin University of China (RUC)](https://www.ruc.edu.cn/), advised by [**Prof. Xin Zhao**](http://ai.ruc.edu.cn/academicfaculty/szdwn/zx/index.htm). My research interests include **Natural Language Processing (NLP)**, **Large Language Models (LLMs)**, and **Agents**, with a particular focus on improving models’ **planning**, **tool use**, and **long-horizon reasoning** in complex real-world tasks.

**My email is: sunshuang@ruc.edu.cn.**

---

## 🔍 Research Interests

My research centers on **LLMs**, **World Models**, and **Agents**. I am especially interested in systematically strengthening the **foundational capabilities** of LLMs and further advancing their generalization and practical utility in complex real-world settings through **LLM-based feedback simulation** and **tool-augmented agent paradigms**.

* **Enhancing foundational LLM capabilities**: I study effective recipes that combine continued pre-training (CPT), supervised fine-tuning (SFT), reinforcement learning (RL), and test-time scaling (TTS) to expand models’ knowledge boundaries and to develop more effective data construction and training strategies.
* **World model learning**: I investigate learnable “surrogate environments” that simulate execution and interaction feedback, enabling models to approximate real environment dynamics at low cost, reducing reliance on heavyweight execution stacks (e.g., containers), and improving scalability.
* **Agent applications and tool use**: I aim to enhance LLMs’ ability to use tools (e.g., web search, code tools, and command-line operations) in realistic workflows, enabling them to solve long-horizon tasks in real-world scenarios.

---

<span class='anchor' id='news'></span>

## 🔥 News

- **[2026-02-04]** We released [**SWE-Master**](https://arxiv.org/pdf/2602.03411) and [**SWE-World**](https://arxiv.org/pdf/2602.03419), aiming to lower the barrier to training code agents and to democratize SWE agent research.  
  - **SWE-Master**: an open, end-to-end post-training pipeline for SWE agents, along with practical enhancements such as **LSP**.  
  - **SWE-World**: an LLM-based surrogate environment that simulates environment feedback, breaking the traditional dependence on heavyweight SWE environments (e.g., Docker) and enabling the first end-to-end **Docker-free** training framework.

- **[2025-05-22]** We released [**SimpleDeepSearcher**](https://aclanthology.org/2025.findings-emnlp.739.pdf): by synthesizing and filtering a small set of high-quality samples for SFT, we substantially improve deep information seeking capability and outperform RL-based methods from the same period.

- **[2025-03-06]** We released [**YuLan-Mini-Instruct**](https://github.com/RUC-GSAI/YuLan-Mini/blob/40a261d3720e08edfbaa1a05a9d90dae7fa1ce85/post_train/README.md): a compact yet strong **2.4B** instruction-tuned model, post-trained from the [YuLan-Mini](https://aclanthology.org/2025.acl-long.268.pdf) base model. Trained efficiently on both open and synthetic data, it achieves competitive performance against mainstream small models such as Qwen2.5-1.5B-Instruct and LLaMA-3.2-3B-Instruct.

---

<span class='anchor' id='publications'></span>

## 📝 Publications

<!-- ===================== SWE-World ===================== -->
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">arXiv 2026</div>
      <img src='images/papers/swe_world.png' alt="SWE-World" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

[**SWE-World: Building Software Engineering Agents in Docker-Free Environments**](https://arxiv.org/pdf/2602.03419)

**Shuang Sun**\*, Huatong Song\*, Lisheng Huang\*, Jinhao Jiang\*, Ran Le, Zhihao Lv, Zongchao Chen, Yiwen Hu, Wenyang Luo, Wayne Xin Zhao†, Yang Song†, Hongteng Xu, Tao Zhang, Ji-Rong Wen  
(\* Equal contribution; † Corresponding)

- We propose **SWE-World**, a Docker-free framework that simulates execution feedback with LLMs, enabling end-to-end training and inference for SWE agents (SFT/RL/TTS) without relying on Docker, thereby substantially lowering the infrastructure barrier.

<!-- Buttons -->
<span class="link-block">
  <a href="https://arxiv.org/pdf/2602.03419" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fas fa-file-pdf"></i></span><span>Paper</span>
  </a>
</span>
<span class="link-block">
  <a href="https://github.com/RUCAIBox/SWE-World" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fab fa-github"></i></span><span>Code</span>
  </a>
</span>
<span class="link-block">
  <a href="TODO_HF_SWE_WORLD" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><span style="font-weight:700;">🤗</span></span><span>HuggingFace</span>
  </a>
</span>
<span class="link-block">
  <a href="https://mp.weixin.qq.com/s/k92yH0pDbYuniHfrwNOYcA" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fab fa-weixin"></i></span><span>WeChat</span>
  </a>
</span>

  </div>
</div>

<!-- ===================== SWE-Master ===================== -->
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">arXiv 2026</div>
      <img src='images/papers/swe_master.png' alt="SWE-Master" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

[**SWE-Master: A Fully Open, End-to-End Post-Training Pipeline for Software Engineering Agents**](https://arxiv.org/pdf/2602.03411)

Huatong Song\*, Lisheng Huang\*, **Shuang Sun**\*, Jinhao Jiang\*, Ran Le, Daixuan Cheng, Guoxin Chen, Yiwen Hu, Zongchao Chen, Wayne Xin Zhao†, Yang Song†, Tao Zhang, Ji-Rong Wen  
(\* Equal contribution; † Corresponding)

- We open-source a fully reproducible end-to-end post-training pipeline for SWE agents (data → long-horizon SFT → RL → TTS), and introduce **LSP**-based structured code navigation to improve interaction efficiency.

<!-- Buttons -->
<span class="link-block">
  <a href="https://arxiv.org/pdf/2602.03411" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fas fa-file-pdf"></i></span><span>Paper</span>
  </a>
</span>
<span class="link-block">
  <a href="https://github.com/RUCAIBox/SWE-Master" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fab fa-github"></i></span><span>Code</span>
  </a>
</span>
<span class="link-block">
  <a href="TODO_HF_SWE_MASTER" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><span style="font-weight:700;">🤗</span></span><span>HuggingFace</span>
  </a>
</span>
<span class="link-block">
  <a href="https://mp.weixin.qq.com/s/k92yH0pDbYuniHfrwNOYcA" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fab fa-weixin"></i></span><span>WeChat</span>
  </a>
</span>

  </div>
</div>

<!-- ===================== SimpleDeepSearcher ===================== -->
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">EMNLP Findings 2025</div>
      <img src='images/papers/simpledeepsearcher.png' alt="SimpleDeepSearcher" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

[**SimpleDeepSearcher: Deep Information Seeking via Web-Powered Reasoning Trajectory Synthesis**](https://aclanthology.org/2025.findings-emnlp.739.pdf)

**Shuang Sun**\*, Huatong Song\*, Yuhao Wang, Ruiyang Ren, Jinhao Jiang, Junjie Zhang, Fei Bai, Jia Deng, Wayne Xin Zhao†, Zheng Liu†, Lei Fang†, Zhongyuan Wang, Ji-Rong Wen  
(\* Equal contribution; † Corresponding)

- We propose a real Web-based data synthesis and multi-criteria curation framework, and show that SFT on only 871 high-quality samples substantially improves deep information seeking capability, outperforming contemporary RL-based approaches.

<!-- Buttons -->
<span class="link-block">
  <a href="https://aclanthology.org/2025.findings-emnlp.739.pdf" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fas fa-file-pdf"></i></span><span>Paper</span>
  </a>
</span>
<span class="link-block">
  <a href="https://github.com/RUCAIBox/SimpleDeepSearcher" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fab fa-github"></i></span><span>Code</span>
  </a>
</span>
<span class="link-block">
  <a href="https://huggingface.co/RUC-AIBOX/QwQ-32B-SimpleDeepSearcher" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><span style="font-weight:700;">🤗</span></span><span>HuggingFace</span>
  </a>
</span>
<span class="link-block">
  <a href="https://mp.weixin.qq.com/s/DWxiU8zeI5ugZgEZxQNp4Q" target="_blank" rel="noopener"
     class="external-link button is-normal is-rounded is-dark">
    <span class="icon"><i class="fab fa-weixin"></i></span><span>WeChat</span>
  </a>
</span>

  </div>
</div>



<span class='anchor' id='honors'></span>

## 🎖 Honors

- **2025** Outstanding Graduate, Northeastern University (**Top 0.9%**)  
- **2023** Huawei Scholarship (**Top 2.3%**)  
- **2022** National Scholarship (**Top 0.2%**)  

---

<span class='anchor' id='educations'></span>

## 📖 Education

- **Sep. 2025 – Present** M.S. student, Gaoling School of Artificial Intelligence, Renmin University of China  
- **Sep. 2021 – Jun. 2025** B.E., School of Computer Science and Engineering, Northeastern University  

---

<span class='anchor' id='internships'></span>

## 💻 Internships

- **Oct. 2025 – Present** Nanbeige LLM Lab, Boss Zhipin
