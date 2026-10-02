---
layout: single
author_profile: true
title: "Research"
permalink: /research/
classes: wide
excerpt: "Research on natural language processing and large language models: benchmarking and evaluation, alignment and bias, and multi-agent systems."
---

I work on natural language processing and large language models, with a focus on how they are trained, fine-tuned, evaluated, and benchmarked. My broader interests include multi-agent systems, alignment and hallucination, and AI4Science. Across projects, I build benchmarks and evaluation pipelines, design multi-agent LLM systems, and test methods that make models more reliable and aligned.
{: .research-lead}

## Current project

<div class="project--current" markdown="1">

### Socio-linguistic modeling to understand the long-term dynamics of news engagement in online media

An NSF Human-Centered Computing (HCC) project in the TulaneAI Group at Tulane University, led by [Aron Culotta](https://www.cs.tulane.edu/~aculotta/). I have worked on it since 2026 as a Graduate Research Assistant.
{: .project-meta}

The project combines natural language processing, large language models, and causal inference to understand how people change their political views and how they approach social interactions on platforms such as Reddit.

So far, I have collected roughly 30,000 public comments and built the preprocessing pipeline, including PII scrubbing and filtering. I also built an LLM annotation system with typed schemas that benchmarks state-of-the-art models against human-coded gold standards on agreement, precision, and recall.

</div>

## Benchmarking and evaluation

Benchmarks shape what we believe a model can do. I build benchmarks and evaluation pipelines, often together with domain experts, to measure where frontier models succeed and where they fail.

<div class="project" markdown="1">
<figure class="project__figure">
  <a href="/assets/images/research/islamic-legal-bench.png"><img src="/assets/images/research/islamic-legal-bench.png" alt="IslamicLegalBench data pipeline from Islamic law books to the final dataset" loading="lazy"></a>
  <figcaption>Questions are drawn from Islamic law books and refined under the supervision of Islamic law experts.</figcaption>
</figure>
<div class="project__text" markdown="1">
<span class="venue-mark venue-mark--journal">Artificial Intelligence and Law, 2026</span>

### IslamicLegalBench

A benchmark of how well LLMs know and reason about Islamic law. It spans 14 task types, from factual recall to advanced jurisprudential reasoning, and draws on legal texts covering more than 1,200 years and several schools of thought. We evaluated GPT-5, Gemini 2.5, Claude 4, DeepSeek R1, Grok 4, and Llama 4 with LLM-as-a-judge scoring, expert human annotation, and zero-shot, few-shot, and chain-of-thought prompting.

[Paper](https://link.springer.com/article/10.1007/s10506-026-09535-4) [arXiv](https://arxiv.org/abs/2602.21226) [Leaderboard](https://huggingface.co/spaces/AbdullahMushtaq/IslamicLegalBench-Leaderboard)
{: .project__links}
</div>
</div>

<div class="project" markdown="1">
<figure class="project__figure">
  <a href="/assets/images/research/can-llms-write.png"><img src="/assets/images/research/can-llms-write.png" alt="Quantitative and qualitative evaluator agents with search and verse-retrieval tools" loading="lazy"></a>
  <figcaption>Quantitative and qualitative evaluator agents use web search and verse-retrieval tools, and their structured outputs go to human evaluators.</figcaption>
</figure>
<div class="project__text" markdown="1">
<span class="venue-mark venue-mark--conference">NeurIPS 2025 Workshop</span>

### Can LLMs Write Faithfully?

An agent-based framework for evaluating religious content written by LLMs. A quantitative agent scores individual essays and a qualitative agent compares responses from several models; both check citations with search tools and return structured analyses for human evaluators. Testing frontier and domain-specific models showed clear gaps in citation accuracy and in faith-sensitive writing.

[arXiv](https://arxiv.org/abs/2510.24438) [Code](https://github.com/AbdullahMushtaq78/Islamic_Writing_HBKU)
{: .project__links}
</div>
</div>

## Alignment and bias

I study how to measure bias in frontier models and how to align their answers so they are more inclusive and reliable.

<div class="project" markdown="1">
<figure class="project__figure">
  <a href="/assets/images/research/worldview-bench.png"><img src="/assets/images/research/worldview-bench.png" alt="Multi-agent multiplex benchmarking pipeline for WorldView-Bench" loading="lazy"></a>
  <figcaption>Perspective-specific agents feed a multiplex agent, whose answers are scored for cultural sentiment and perspective distribution.</figcaption>
</figure>
<div class="project__text" markdown="1">
<span class="venue-mark venue-mark--journal">JAIR, 2026</span>

### WorldView-Bench

A benchmark of 175 questions in 7 categories for evaluating global cultural perspectives in LLMs. In our multiplex approach, perspective-specific agents answer in parallel and a multiplex agent combines their views. This raised inclusivity from 13% to 94% and reduced negative sentiment to 2.4%.

[Paper](https://doi.org/10.1613/jair.1.19001) [arXiv](http://arxiv.org/abs/2505.09595) [Code](https://github.com/AbdullahMushtaq78/WorldView-Bench)
{: .project__links}
</div>
</div>

<div class="project" markdown="1">
<figure class="project__figure">
  <a href="/assets/images/research/cultural-bias.png"><img src="/assets/images/research/cultural-bias.png" alt="Overview of cultural polarization in LLM answers on educational topics" loading="lazy"></a>
  <figcaption>We analyze both what LLMs say about educational topics and how they say it.</figcaption>
</figure>
<div class="project__text" markdown="1">
<span class="venue-mark venue-mark--conference">IEEE EDUCON 2025</span>

### Auditing frontier LLMs for cultural bias

An audit of cultural bias in GPT-4, Claude 3.5, Llama 3.1 and 3.2, and Mistral 7B on educational topics. Bias-aware prompt calibration, controlled generation, and multi-agent systems raised inclusivity rates from 3.25% to 98%.

[arXiv](https://arxiv.org/abs/2501.03259)
{: .project__links}
</div>
</div>

## Multi-agent systems

I build multi-agent LLM systems in which coordinator and specialist agents split complex judgments into smaller checks, and I compare their verdicts with those of human experts.

<div class="project" markdown="1">
<figure class="project__figure">
  <a href="/assets/images/research/masc.png"><img src="/assets/images/research/masc.png" alt="MASC architecture with a coordinator agent and eight specialist agents" loading="lazy"></a>
  <figcaption>A coordinator agent splits a project proposal into tasks for eight specialist evaluation agents.</figcaption>
</figure>
<div class="project__text" markdown="1">
<span class="venue-mark venue-mark--conference">IEEE EDUCON 2025</span>

### MASC, a multi-agent co-pilot for senior design projects

A co-pilot that helps assess engineering senior design projects. Eight specialist agents evaluate problem formulation, system complexity, ethics, risk, and methodology, alongside NLP measures such as lexical cohesion and clause density. Their combined assessment matched expert faculty evaluations 89% of the time.

[arXiv](https://arxiv.org/abs/2501.01205) [Code](https://github.com/AbdullahMushtaq78/Multi-Agent-SDP-Copliot)
{: .project__links}
</div>
</div>

<div class="project" markdown="1">
<figure class="project__figure">
  <a href="/assets/images/research/slr-gpt.png"><img src="/assets/images/research/slr-gpt.png" alt="SLR-GPT architecture with PRISMA-inspired multi-agent societies" loading="lazy"></a>
  <figcaption>PRISMA-inspired multi-agent societies evaluate a systematic review end to end, from PDF parsing to a web interface.</figcaption>
</figure>
<div class="project__text" markdown="1">
<span class="venue-mark venue-mark--preprint">Preprint, 2025</span>

### SLR-GPT: can agents judge systematic reviews like humans?

Twenty-seven LLM agents, organized into PRISMA-inspired deliberative societies, evaluate a systematic literature review from a single PDF. The system combines few-shot prompting, tool use, vision-language models, and arXiv access, and agreed with domain experts 84% of the time on reviews in medicine, AI, and AR/VR. This is joint work with Weill Cornell Medicine and Qatar University.

[arXiv](https://arxiv.org/abs/2509.17240)
{: .project__links}
</div>
</div>

## Earlier work

Before focusing on LLMs, I worked on human-computer interaction, language technology for a low-resource language, and 3D computer vision.

<div class="earlier" markdown="1">
<div markdown="1">
### Immersive learning with VR

At Virtuality Labs, ITU, I led a team of junior researchers in designing and running Pakistan's first VR classroom field experiment, comparing VR, face-to-face, and Zoom teaching with more than 100 first-year CS students. The study was published at [ECIS 2025](https://aisel.aisnet.org/ecis2025/education/education/1/).
</div>
<div markdown="1">
### Urdu NLP for mental health

At the CSaLT Lab, LUMS, with Imperial College London, I fine-tuned and integrated Whisper, BERT, MuRIL, and GPT-2 on a custom Urdu dataset to build an Urdu-language psychotherapy chatbot.
</div>
<div markdown="1">
### 3D reconstruction

At the Intelligent Machines Lab, ITU, in a joint project with ETRI (South Korea), I built a synthetic 4D dataset of more than 80 indoor scenes (about 2 TB) in Unity3D and benchmarked SfM, COLMAP, NeRF, and 3D Gaussian Splatting.
</div>
</div>

All papers, with links to code and data, are on the [Publications](/publications/) page, and my full record is in my [CV](/assets/pdf/cv.pdf).
