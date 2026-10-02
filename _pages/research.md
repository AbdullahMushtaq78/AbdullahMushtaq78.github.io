---
layout: single
author_profile: true
title: "Research"
permalink: /research/
classes: wide
excerpt: "Research on applied NLP and large language models: benchmarking and evaluation, cultural alignment, and multi-agent LLM systems."
---

My research focuses on applied natural language processing and large language models (LLMs), with an emphasis on how these models are trained, fine-tuned, evaluated, and benchmarked. I am particularly interested in settings where cultural, religious, legal, or political context decides what a good answer looks like, and where mistakes carry real consequences. My work builds rigorous benchmarks and evaluation pipelines, designs multi-agent LLM systems, and studies how to make model behavior more aligned, inclusive, and reliable.
{: .research-lead}

<div class="research-tags">
  <span class="research-tag">Natural Language Processing</span>
  <span class="research-tag">Large Language Models</span>
  <span class="research-tag">Multi-Agent Systems</span>
  <span class="research-tag">Alignment and Hallucination</span>
  <span class="research-tag">AI4Science</span>
</div>

<div class="research-current" markdown="1">
<span class="research-eyebrow">Current research · NSF-HCC</span>

### Socio-linguistic modeling to understand the long-term dynamics of news engagement in online media

Tulane University · TulaneAI Group · PI: [Aron Culotta](https://www.cs.tulane.edu/~aculotta/) · 2026 – present
{: .research-meta}

As a Graduate Research Assistant in the TulaneAI Group, I work on this NSF Human-Centered Computing (HCC) project, which combines natural language processing, large language models, and causal inference to understand how people change their political views and how they approach social interactions on platforms such as Reddit.

So far, I have collected roughly 30,000 public comments and built the preprocessing pipeline, including PII scrubbing and filtering. I also built an LLM annotation system with typed schemas that benchmarks state-of-the-art models against human-coded gold standards on agreement, precision, and recall.

- **~30k** public comments
- **LLM annotation** with typed schemas
- **Benchmarked** against human-coded gold standards
{: .research-stats}
</div>

<p class="research-kicker">Research theme 1</p>

## Benchmarking LLMs in Culturally and Legally Grounded Domains

Standard benchmarks rarely capture how LLMs behave when religion, law, or culture defines what a correct answer is. Together with domain experts, I build domain-specific benchmarks and evaluation pipelines that show where frontier models succeed and where they fail.

<article class="research-card" data-type="journal" markdown="1">
<figure class="research-card__figure">
  <a href="/assets/images/research/islamic-legal-bench.png"><img src="/assets/images/research/islamic-legal-bench.png" alt="IslamicLegalBench data pipeline from Islamic law books to the final dataset" loading="lazy"></a>
  <figcaption>Questions are drawn from Islamic law books and refined under the supervision of Islamic law experts.</figcaption>
</figure>
<div class="research-card__body" markdown="1">
<span class="research-badge">AI &amp; Law 2026</span>

### IslamicLegalBench

A benchmark for evaluating how well LLMs know and reason about Islamic law. It spans 14 task types, from factual recall to advanced jurisprudential reasoning, and draws on legal texts covering more than 1,200 years and multiple schools of thought. We evaluated frontier models including GPT-5, Gemini 2.5, Claude 4, DeepSeek R1, Grok 4, and Llama 4 using LLM-as-a-judge scoring, expert human annotation, and zero-shot, few-shot, and chain-of-thought prompting.

- **14** task types
- **1,200+ years** of legal tradition
- **6** frontier models
{: .research-stats}

[<i class="fas fa-book-open" aria-hidden="true"></i> Paper](https://link.springer.com/article/10.1007/s10506-026-09535-4){: .pub-link} [<i class="fas fa-file-alt" aria-hidden="true"></i> arXiv](https://arxiv.org/abs/2602.21226){: .pub-link} [<i class="fas fa-trophy" aria-hidden="true"></i> Leaderboard](https://huggingface.co/spaces/AbdullahMushtaq/IslamicLegalBench-Leaderboard){: .pub-link}
{: .research-card__links}
</div>
</article>

<article class="research-card" data-type="conference" markdown="1">
<figure class="research-card__figure">
  <a href="/assets/images/research/can-llms-write.png"><img src="/assets/images/research/can-llms-write.png" alt="Quantitative and qualitative evaluator agents with search and verse-retrieval tools" loading="lazy"></a>
  <figcaption>Quantitative and qualitative evaluator agents use web search and verse-retrieval tools, and their structured outputs go to human evaluators.</figcaption>
</figure>
<div class="research-card__body" markdown="1">
<span class="research-badge">NeurIPS 2025 Workshop</span>

### Can LLMs Write Faithfully?

An agent-based framework for evaluating religious content written by LLMs. A quantitative agent scores individual essays and a qualitative agent compares responses from several models; both verify citations with search tools and return structured analyses for human evaluators. Benchmarking frontier and domain-specific models revealed critical gaps in citation accuracy and faith-sensitive content generation.

- **Dual-agent** evaluation
- **Citation** verification
{: .research-stats}

[<i class="fas fa-file-alt" aria-hidden="true"></i> arXiv](https://arxiv.org/abs/2510.24438){: .pub-link} [<i class="fab fa-github" aria-hidden="true"></i> Code](https://github.com/AbdullahMushtaq78/Islamic_Writing_HBKU){: .pub-link}
{: .research-card__links}
</div>
</article>

<p class="research-kicker">Research theme 2</p>

## Cultural Alignment and Inclusive AI

LLMs increasingly shape how students and the public learn about the world, so whose perspective they present matters. I study how to measure cultural bias in frontier models and how to steer them toward answers that represent many worldviews.

<article class="research-card" data-type="journal" markdown="1">
<figure class="research-card__figure">
  <a href="/assets/images/research/worldview-bench.png"><img src="/assets/images/research/worldview-bench.png" alt="Multi-agent multiplex benchmarking pipeline for WorldView-Bench" loading="lazy"></a>
  <figcaption>Perspective-specific agents feed a multiplex agent, whose answers are scored for cultural sentiment and perspective distribution.</figcaption>
</figure>
<div class="research-card__body" markdown="1">
<span class="research-badge">JAIR 2026</span>

### WorldView-Bench

A benchmark of 175 questions across 7 categories for evaluating global cultural perspectives in LLMs. In our multiplex approach, perspective-specific agents answer in parallel and a multiplex agent combines their views, which raised inclusivity from 13% to 94% and reduced negative sentiment to 2.4%.

- **175** questions, **7** categories
- Inclusivity **13% → 94%**
- Negative sentiment **2.4%**
{: .research-stats}

[<i class="fas fa-book-open" aria-hidden="true"></i> Paper](https://doi.org/10.1613/jair.1.19001){: .pub-link} [<i class="fas fa-file-alt" aria-hidden="true"></i> arXiv](http://arxiv.org/abs/2505.09595){: .pub-link} [<i class="fab fa-github" aria-hidden="true"></i> Code](https://github.com/AbdullahMushtaq78/WorldView-Bench){: .pub-link}
{: .research-card__links}
</div>
</article>

<article class="research-card" data-type="conference" markdown="1">
<figure class="research-card__figure">
  <a href="/assets/images/research/cultural-bias.png"><img src="/assets/images/research/cultural-bias.png" alt="Overview of cultural polarization in LLM answers on educational topics" loading="lazy"></a>
  <figcaption>We analyze both what LLMs say about educational topics and how they say it.</figcaption>
</figure>
<div class="research-card__body" markdown="1">
<span class="research-badge">IEEE EDUCON 2025</span>

### Auditing and Aligning Frontier LLMs for Cultural Bias

An audit of cultural bias in frontier LLMs, including GPT-4, Claude 3.5, Llama 3.1 and 3.2, and Mistral 7B, on educational topics. Bias-aware prompt calibration, controlled generation, and multi-agent systems raised inclusivity rates from 3.25% to 98%.

- Inclusivity **3.25% → 98%**
{: .research-stats}

[<i class="fas fa-file-alt" aria-hidden="true"></i> arXiv](https://arxiv.org/abs/2501.03259){: .pub-link}
{: .research-card__links}
</div>
</article>

<p class="research-kicker">Research theme 3</p>

## Multi-Agent LLM Systems

Some judgments are too complex for a single prompt. I design multi-agent systems in which coordinator, task, and specialist agents break an evaluation into smaller, checkable steps, and I measure how closely their judgments match those of human experts.

<article class="research-card" data-type="conference" markdown="1">
<figure class="research-card__figure">
  <a href="/assets/images/research/masc.png"><img src="/assets/images/research/masc.png" alt="MASC architecture with a coordinator agent and eight specialist agents" loading="lazy"></a>
  <figcaption>A coordinator agent splits a project proposal into tasks for eight specialist evaluation agents.</figcaption>
</figure>
<div class="research-card__body" markdown="1">
<span class="research-badge">IEEE EDUCON 2025</span>

### MASC: A Multi-Agent Co-Pilot for Senior Design Projects

A multi-agent co-pilot that helps assess senior design projects in engineering. Specialist agents evaluate problem formulation, system complexity, ethics, risk, and methodology, alongside NLP metrics such as lexical cohesion and clause density. Their combined assessment reached 89% alignment with expert faculty evaluations.

- **8** specialist agents
- **89%** alignment with faculty
{: .research-stats}

[<i class="fas fa-file-alt" aria-hidden="true"></i> arXiv](https://arxiv.org/abs/2501.01205){: .pub-link} [<i class="fab fa-github" aria-hidden="true"></i> Code](https://github.com/AbdullahMushtaq78/Multi-Agent-SDP-Copliot){: .pub-link}
{: .research-card__links}
</div>
</article>

<article class="research-card" data-type="preprint" markdown="1">
<figure class="research-card__figure">
  <a href="/assets/images/research/slr-gpt.png"><img src="/assets/images/research/slr-gpt.png" alt="SLR-GPT architecture with PRISMA-inspired multi-agent societies" loading="lazy"></a>
  <figcaption>PRISMA-inspired multi-agent societies evaluate a systematic review end to end, from PDF parsing to a web interface.</figcaption>
</figure>
<div class="research-card__body" markdown="1">
<span class="research-badge">Preprint 2025</span>

### SLR-GPT: Can Agents Judge Systematic Reviews Like Humans?

A system of 27 specialized LLM agents, organized into PRISMA-inspired deliberative societies, that evaluates a systematic literature review from a single PDF. It combines few-shot prompting, tool use, vision-language models, and arXiv access, and reached 84% agreement with domain experts on reviews in medicine, AI, and AR/VR. This work is a collaboration with Weill Cornell Medicine and Qatar University.

- **27** agents
- **84%** agreement with experts
{: .research-stats}

[<i class="fas fa-file-alt" aria-hidden="true"></i> arXiv](https://arxiv.org/abs/2509.17240){: .pub-link}
{: .research-card__links}
</div>
</article>

## Earlier Work

Before focusing on LLMs, I worked on human-computer interaction, language technology for low-resource languages, and 3D computer vision.

<div class="research-earlier">
  <div class="research-earlier__item">
    <i class="fas fa-vr-cardboard" aria-hidden="true"></i>
    <h4>Immersive Learning with VR</h4>
    <p>At Virtuality Labs, ITU, I led a team of junior researchers in designing and running Pakistan's first VR classroom field experiment, comparing VR, face-to-face, and Zoom teaching with more than 100 first-year CS students. The study was published at <a href="https://aisel.aisnet.org/ecis2025/education/education/1/">ECIS 2025</a> and covered on national TV.</p>
  </div>
  <div class="research-earlier__item">
    <i class="fas fa-comments" aria-hidden="true"></i>
    <h4>Low-Resource NLP for Mental Health</h4>
    <p>At the CSaLT Lab, LUMS, in collaboration with Imperial College London, I fine-tuned and integrated models such as Whisper, BERT, MuRIL, and GPT-2 on a custom Urdu dataset to build an Urdu-language psychotherapy chatbot.</p>
  </div>
  <div class="research-earlier__item">
    <i class="fas fa-cube" aria-hidden="true"></i>
    <h4>3D Reconstruction and Neural Rendering</h4>
    <p>At the Intelligent Machines Lab, ITU, in a joint project with ETRI (South Korea), I built a synthetic 4D dataset of more than 80 indoor scenes (about 2 TB) in Unity3D and benchmarked reconstruction with SfM, COLMAP, NeRF, and 3D Gaussian Splatting.</p>
  </div>
</div>

<div class="research-cta" markdown="1">
The full list of papers, with links to code and data, is on my Publications page.

[View all publications](/publications/){: .btn .btn--primary} [Download CV](/assets/pdf/cv.pdf){: .btn .btn--inverse}
</div>
