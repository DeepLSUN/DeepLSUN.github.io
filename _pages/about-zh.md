---
permalink: /zh/
lang: zh
title: "Shuang Sun"
excerpt: "M.S. student at Gaoling School of Artificial Intelligence (RUC). Research: NLP, LLMs, and Agents / 中国人民大学高瓴人工智能学院硕士：NLP、大语言模型与智能体。"
author_profile: true
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

## 👋 关于我

我目前是[中国人民大学](https://www.ruc.edu.cn/)[高瓴人工智能学院（GSAI）](http://ai.ruc.edu.cn/)硕士一年级研究生，导师为[**赵鑫教授**](http://ai.ruc.edu.cn/academicfaculty/szdwn/zx/index.htm)。我的研究兴趣包括**自然语言处理（NLP）**、**大语言模型（LLMs）**与**智能体（Agents）**，尤其关注如何提升模型在复杂任务中的规划、工具使用与长程推理能力。

**我的邮箱是：sunshuang@ruc.edu.cn.**



---

## 🔍 研究兴趣

我的研究聚焦于**大语言模型（LLMs）**、**世界模型（World Models）**与**智能体（Agents）**。我特别关注如何系统性提升大语言模型的**基础能力**，并进一步通过**基于 LLM 的反馈模拟**与**工具增强的智能体范式**，推动模型在真实复杂任务中的泛化与可用性。

* **增强大语言模型基础能力**：结合持续预训练（CPT）、监督微调（SFT）、强化学习（RL）与测试时扩展（TTS），拓宽模型的知识边界，并探索更有效的数据构造与训练策略。
* **世界模型建模**：研究可学习的“替代环境”以模拟执行与交互反馈，使模型能够在低成本条件下近似真实环境动态，从而降低对重型执行环境的依赖并提升可扩展性。
* **智能体应用与工具使用**：提升模型在真实工作流中调用工具（如搜索、代码调用与命令行操作）的能力，使其能够解决真实场景下的长程任务。


---

<span class='anchor' id='news'></span>

## 🔥 最新动态

- **[2026-02-04]** 我们发布了 [**SWE-Master**](https://arxiv.org/pdf/2602.03411)与 [**SWE-World**](https://arxiv.org/pdf/2602.03419)，目标是降低代码智能体训练门槛、推动代码智能体研究平民化。  
  - SWE-Master：开放端到端的 SWE Agents 后训练流水线，并探索了如 **LSP** 等增强技巧。  
  - SWE-World：基于大语言模型模拟环境反馈，突破传统 SWE 重环境（Docker）限制，实现首个全流程 **Docker-free** 训练框架。  

- **[2025-05-22]** 发布 [**SimpleDeepSearcher**](https://aclanthology.org/2025.findings-emnlp.739.pdf)：通过数据合成与筛选获得少量高质量数据进行 SFT，显著提升模型深度搜索能力，并超过同期基于 RL 的方法。  

- **[2025-03-06]** 发布 [**YuLan-Mini-Instruct**](https://github.com/RUC-GSAI/YuLan-Mini/blob/40a261d3720e08edfbaa1a05a9d90dae7fa1ce85/post_train/README.md)：一个 **2.4B** 轻量但强大的指令模型，是 [YuLan-Mini](https://aclanthology.org/2025.acl-long.268.pdf) 基座的后训练版本，在开源+合成数据上高效训练，表现可对标 Qwen2.5-1.5B-Instruct、LLama-3.2-3B-Instruct 等主流小模型。  

---
<span class='anchor' id='publications'></span>

## 📝 论文

<!-- ===================== SWE-World ===================== -->
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">arXiv 2026</div>
      <img src="{{ '/images/papers/swe_world.png' | relative_url }}" alt="SWE-World" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

[**SWE-World: Building Software Engineering Agents in Docker-Free Environments**](https://arxiv.org/pdf/2602.03419)

**Shuang Sun**\*, Huatong Song\*, Lisheng Huang\*, Jinhao Jiang\*, Ran Le, Zhihao Lv, Zongchao Chen, Yiwen Hu, Wenyang Luo, Wayne Xin Zhao†, Yang Song†, Hongteng Xu, Tao Zhang, Ji-Rong Wen  
(\* Equal contribution; † Corresponding)

- 提出了 **SWE-World** 框架，通过 LLMs 模拟执行反馈，实现了无需 Docker 的 SWE Agent 全流程训练与推理（SFT/RL/TTS），显著降低了研究门槛。

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
      <img src="{{ '/images/papers/swe_master.png' | relative_url }}" alt="SWE-Master" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

[**SWE-Master: A Fully Open, End-to-End Post-Training Pipeline for Software Engineering Agents**](https://arxiv.org/pdf/2602.03411)

Huatong Song\*, Lisheng Huang\*, **Shuang Sun**\*, Jinhao Jiang\*, Ran Le, Daixuan Cheng, Guoxin Chen, Yiwen Hu, Zongchao Chen, Wayne Xin Zhao†, Yang Song†, Tao Zhang, Ji-Rong Wen  
(\* Equal contribution; † Corresponding)

- 开源 SWE 智能体端到端后训练流水线（数据→长程SFT→RL→TTS），并引入 LSP 级代码导航提升交互效率。

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
      <img src="{{ '/images/papers/simpledeepsearcher.png' | relative_url }}" alt="SimpleDeepSearcher" width="100%">
    </div>
  </div>

  <div class='paper-box-text' markdown="1">

[**SimpleDeepSearcher: Deep Information Seeking via Web-Powered Reasoning Trajectory Synthesis**](https://aclanthology.org/2025.findings-emnlp.739.pdf)

**Shuang Sun**\*, Huatong Song\*, Yuhao Wang, Ruiyang Ren, Jinhao Jiang, Junjie Zhang, Fei Bai, Jia Deng, Wayne Xin Zhao†, Zheng Liu†, Lei Fang†, Zhongyuan Wang, Ji-Rong Wen  
(\* Equal contribution; † Corresponding)

- 提出了基于真实 Web 搜索环境的数据合成与多维筛选框架，仅用 871 条高质量 SFT 样本显著提升深度搜索能力，超越同期 RL 方法。

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

## 🎖 荣誉

- **2025** 东北大学优秀毕业生（Top 0.9%）  
- **2023** 华为奖学金（Top 2.3%）  
- **2022** 国家奖学金（Top 0.2%）  

---

<span class='anchor' id='educations'></span>

## 📖 教育经历

- **2025.09 – 至今** 中国人民大学，高瓴人工智能学院，硕士  
- **2021.09 – 2025.06** 东北大学，计算机科学与工程学院，本科  

---

<span class='anchor' id='internships'></span>

## 💻 实习经历

- **2025.10 – 至今** Nanbeige LLM Lab, Boss Zhipin
