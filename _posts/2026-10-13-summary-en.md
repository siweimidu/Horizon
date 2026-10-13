---
layout: default
title: "Horizon Summary: 2026-10-13 (EN)"
date: 2026-10-13
lang: en
---

> From 125 items, 13 important content pieces were selected

---

**Technology News**
1. [Ai2&\#x27;s byte-level language model architecture Bolmo published in Nature](#item-tech-news-1) ⭐️ 9.0/10
2. [Repurposing WiFi 7 Router Chipsets as 320Msps SDR Receivers](#item-tech-news-2) ⭐️ 8.0/10
3. [Meta Releases Muse Wonder AI Models with New Agentic Capabilities](#item-tech-news-3) ⭐️ 8.0/10
4. [Meta Deploys Media over QUIC for Instagram Live Ingestion](#item-tech-news-4) ⭐️ 8.0/10
5. [Microsoft Research Introduces StudentSim for AI Tutoring Evaluation](#item-tech-news-5) ⭐️ 8.0/10
6. [NVIDIA 论文提出在首个让测试通过的编辑处评估 base 模型，预测编码智能体后训练表现](#item-tech-news-6) ⭐️ 8.0/10
7. [微软计划到 2027 年将自研 Maia AI 芯片扩展至吉瓦级规模](#item-tech-news-7) ⭐️ 8.0/10
8. [Introducing Olmo-core 3: Open, scalable training infrastructure for large MoEs](#item-tech-news-8) ⭐️ 8.0/10
9. [Qwen Releases QwenGyre Framework for Long-Horizon AI Agent Training](#item-tech-news-9) ⭐️ 8.0/10
10. [AMD Launches Helion AI Rack System Supporting Up to 32,000 CPU Cores](#item-tech-news-10) ⭐️ 8.0/10
11. [Mistral AI Releases Le Chonk Model for Visual Grounding](#item-tech-news-11) ⭐️ 7.0/10
12. [Allen Institute for AI releases open-weights AstaBrief model](#item-tech-news-12) ⭐️ 7.0/10
13. [Yann LeCun Argues World Models, Not LLMs, Are Key to Future AI Breakthroughs](#item-tech-news-13) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Ai2&\#x27;s byte-level language model architecture Bolmo published in Nature](https://allenai.org/blog/bolmo-nature) ⭐️ 9.0/10

The Allen Institute for AI \(Ai2\) has published its research on Bolmo, a fully open-source language model architecture that operates directly on raw bytes, in the journal Nature. By eliminating traditional tokenization, this approach allows models to process data without the vocabulary constraints and inefficiencies inherent in subword-based systems.

rss · Ai2 News · Oct 31, 00:00

**「Context for Byte-Level Modeling」** Most large language models rely on subword tokenization, which maps text to fixed vocabularies and can struggle with non-standard data or multilingual text. Bolmo addresses this by using a two-stage conversion process to retrofit existing subword-based models into byte-level architectures, allowing them to process raw data directly while maintaining competitive performance.

**「Elimination of Tokenization Constraints」** By operating directly on raw bytes rather than subword tokens, Bolmo removes the linguistic biases and arithmetic limitations inherent in traditional tokenization methods, potentially improving performance on tasks involving non-English languages or complex character-level manipulation.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2512.15586">Bolmo: Byteifying the Next Generation of Language Models</a></li>
<li><a href="https://arxiv.org/abs/2512.15586">[2512.15586] Bolmo: Byteifying the Next Generation of ... Now in Nature: Retrofitting language models to operate over ... Introducing Bolmo: Byteifying the next generation of language ... Now in Nature: Retrofitting language models to operate over… Ai2&#x27;s byte-level Bolmo research published in Nature, new ...</a></li>
<li><a href="https://crazyrouter.com/en/blog/tokens-vs-bytes-what-llms-actually-see">Tokens vs Bytes in AI: What LLMs Actually See When You Type</a></li>
<li><a href="https://letsdatascience.com/blog/tokenization-deep-dive-why-it-matters-more-than-you-think">How LLM Tokenization Actually Works Under the Hood</a></li>

</ul>
</details>

**Tags**: `#Artificial Intelligence`, `#Language Models`, `#Machine Learning`, `#Research`, `#Open Source`

---

<a id="item-tech-news-2"></a>
### [Repurposing WiFi 7 Router Chipsets as 320Msps SDR Receivers](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

A developer has released a project that repurposes WiFi 7 router chipsets to function as software-defined radio \(SDR\) receivers capable of 320Msps sampling. This implementation allows consumer-grade networking hardware to perform wideband signal analysis in the 5 GHz spectrum. The project provides a low-cost alternative to dedicated wideband SDR equipment for hobbyists and researchers.

hackernews · djfergus · Oct 12, 12:41 · [Discussion](https://news.ycombinator.com/item?id=50055593)

**「WiFi 7 Hardware Architecture」** The Gemtek W1700K router utilizes the MediaTek MT7996 wireless chipset, which supports the high-bandwidth requirements of the WiFi 7 \(802.11be\) standard. This chipset is paired with the Airoha AN7581 SoC, a platform that has recently become a target for custom OpenWrt firmware development to enable advanced networking and signal processing capabilities.

**「Impact」** Users can now access high-bandwidth signal analysis at a significantly lower cost than traditional SDR hardware, with potential compatibility extending to devices like the Banana Pi R4 that share the same WiFi 7 chipset.

**「Community Discussion」** Commenters expressed enthusiasm for the project&\#x27;s cost-effectiveness, noting that while it is not a general-purpose receiver, it offers an unprecedented price-to-performance ratio for 5 GHz analysis. Some users suggested that adding an upconverter could further expand the hardware&\#x27;s utility into a 4 GHz communications service monitor.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/h0m3us3r/w1700k-sdr">GitHub - h0m3us3r/w1700k-sdr</a></li>
<li><a href="https://github.com/Gilly1970/Gemtek-W1700K">GitHub - Gilly1970/Gemtek-W1700K</a></li>

</ul>
</details>

**Tags**: `#software-defined-radio`, `#wifi-7`, `#hardware-hacking`, `#signal-processing`, `#embedded-systems`

---

<a id="item-tech-news-3"></a>
### [Meta Releases Muse Wonder AI Models with New Agentic Capabilities](https://research.meta.ai/blog/muse-wonder) ⭐️ 8.0/10

Meta has launched the Muse Wonder and Muse Wonder Full AI models, designed for expert tasks in fields such as law, finance, and healthcare. The models introduce Active Memory for cross-conversation information retention and Active Focus for error-handling and user-verification workflows. Access is available through Muse subscriptions, with pricing tiers ranging from $20 to $200 per month depending on the model version and feature set.

hackernews · meetpateltech · Oct 12, 16:48 · [Discussion](https://news.ycombinator.com/item?id=50059115)

**「Context for Muse Wonder」** Muse Wonder builds upon the Muse platform, which Meta introduced in September 2026 as a personal AI agent designed to perform tasks across third-party applications and social media services. Unlike standard chatbots, the original Muse was developed to act as a digital assistant capable of executing multi-step workflows and managing user projects.

**「Impact」** The introduction of Muse Wonder marks a shift in Meta&\#x27;s commercial strategy, as the higher subscription pricing suggests the company is positioning its models as premium, frontier-level competitors rather than discounted alternatives to existing industry leaders.

**「Community Discussion」** Users noted that the model&\#x27;s performance appears competitive with top-tier alternatives like Claude 3 Opus, with some commenters suggesting that Meta&\#x27;s move toward higher pricing signals confidence in the model&\#x27;s capabilities. Others expressed a desire for Meta to release the model weights to further increase competition among frontier AI developers.

<details><summary>References</summary>
<ul>
<li><a href="https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/">Introducing Muse : The World’s First Personal AI Agent Built for Everyone</a></li>
<li><a href="https://www.nytimes.com/2026/09/08/technology/meta-muse-ai-agent.html">Meta Introduces Muse , an A . I . Agent That Can Send Your Emails and...</a></li>

</ul>
</details>

**Tags**: `#Artificial Intelligence`, `#Meta`, `#Large Language Models`, `#AI Industry`, `#Model Benchmarking`

---

<a id="item-tech-news-4"></a>
### [Meta Deploys Media over QUIC for Instagram Live Ingestion](https://aihot.news/items/d7nio8hwc8iydg46m4dyqig8g) ⭐️ 8.0/10

Meta has transitioned Instagram Live video ingestion on iOS and Android to the Media over QUIC \(MoQ\) protocol. This deployment represents one of the largest known production applications of the open-standard transport protocol to date.

rss · AIHOT 全站 · Oct 12, 16:01

**「Background」** Media over QUIC is an emerging open standard designed to provide low-latency media transport by leveraging the QUIC transport protocol. It aims to replace older, less efficient streaming protocols by reducing handshake overhead and improving performance over unstable network conditions.

**「Impact」** By adopting MoQ, Meta can achieve lower latency and improved reliability for live video ingestion, potentially enhancing the real-time interaction experience for Instagram Live creators and viewers.

**Tags**: `#Media over QUIC`, `#Video Engineering`, `#Networking`, `#Meta`, `#Streaming`

---

<a id="item-tech-news-5"></a>
### [Microsoft Research Introduces StudentSim for AI Tutoring Evaluation](https://aihot.news/items/e1o7hw5u4t6988ntb2i2p43zf) ⭐️ 8.0/10

Microsoft Research has introduced StudentSim, a research framework that uses de-identified learning records to simulate personalized student behavior for testing AI tutoring systems. The system includes the StudentSimEval benchmark, which evaluates simulation fidelity and instructional responsiveness across chess, English writing, and mathematics. StudentSim is intended strictly as a research tool for pre-deployment evaluation and is not designed for classroom use or as a replacement for human educators.

rss · AIHOT 全站 · Oct 12, 16:00

**「Background」** Developing AI tutoring systems typically requires extensive testing with real students, which presents logistical challenges and potential risks to the learning experience. StudentSim addresses this bottleneck by providing a controlled, simulated environment to iterate on AI performance before live deployment.

**「Impact」** Developers of AI-driven educational tools can now utilize the StudentSimEval benchmark to quantitatively assess their systems&\#x27; instructional effectiveness and behavioral accuracy, potentially reducing the reliance on early-stage human trials.

**Tags**: `#AI Research`, `#EdTech`, `#Machine Learning`, `#Simulation`, `#Microsoft`

---

<a id="item-tech-news-6"></a>
### [NVIDIA 论文提出在首个让测试通过的编辑处评估 base 模型，预测编码智能体后训练表现](https://aihot.news/items/h0g8pz7j7qx8xdjxhuan75vq2) ⭐️ 8.0/10

NVIDIA researchers propose a new evaluation method that predicts the post-training performance of coding agents by assessing base models at the first successful edit point, showing a high correlation with SWE-bench Verified scores.

rss · AIHOT 全站 · Oct 12, 15:39

**Tags**: `#AI Agents`, `#Software Engineering`, `#LLM Evaluation`, `#NVIDIA`, `#Machine Learning`

---

<a id="item-tech-news-7"></a>
### [微软计划到 2027 年将自研 Maia AI 芯片扩展至吉瓦级规模](https://aihot.news/items/x3u8gm84b20vqg1lsnmwsvrbu) ⭐️ 8.0/10

Microsoft plans to scale its proprietary Maia AI chips to gigawatt levels by 2027 to power its core AI services, citing superior energy efficiency compared to standard GPUs.

rss · AIHOT 全站 · Oct 12, 15:24

**Tags**: `#Microsoft`, `#AI Hardware`, `#Cloud Infrastructure`, `#Maia Chips`, `#Inference`

---

<a id="item-tech-news-8"></a>
### [Introducing Olmo-core 3: Open, scalable training infrastructure for large MoEs](https://allenai.org/blog/olmocore3) ⭐️ 8.0/10

Ai2 has released Olmo-core 3, an open-source training infrastructure designed to improve the efficiency and scalability of training large Mixture-of-Experts models.

rss · Ai2 News · Oct 31, 00:00

**Tags**: `#Artificial Intelligence`, `#Machine Learning`, `#Open Source`, `#Distributed Systems`, `#MoE`

---

<a id="item-tech-news-9"></a>
### [Qwen Releases QwenGyre Framework for Long-Horizon AI Agent Training](https://www.reddit.com/gallery/1x41myz) ⭐️ 8.0/10

Qwen has released QwenGyre, an elastic reinforcement learning framework designed to optimize the training of AI agents on extremely long-horizon tasks. The framework features an elastic scheduler that dynamically reallocates GPU resources during live execution and a trajectory processor that utilizes prefix-shared trees to deduplicate training samples. In testing with the Qwen3.8-2.4T-A95B model, QwenGyre achieved a 44% reduction in end-to-end training time and improved NL2RepoBench scores from 52.5% to 58.5%.

reddit · r/LocalLLaMA · ResearchCrafty1804 · Oct 12, 13:18 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1x41myz/qwen_released_qwengyre_rl_framework_for_training/)

**「Background」** Training AI agents for long-horizon tasks typically involves managing complex, branching execution paths that are computationally expensive and difficult to parallelize. Traditional reinforcement learning setups often struggle with these tasks due to inefficient resource allocation and redundant data processing during rollout and training phases.

**「Impact」** Researchers and developers working on agentic AI can expect significantly faster iteration cycles and improved performance on complex, multi-step benchmarks by adopting QwenGyre&\#x27;s elastic scheduling and trajectory processing architecture.

**「Community Discussion」** Community members expressed excitement over the framework&\#x27;s efficiency, while several users noted that the accompanying research paper frequently references the Qwen3.6-122B model, fueling speculation about its potential release.

**Tags**: `#Reinforcement Learning`, `#AI Agents`, `#Distributed Systems`, `#Qwen`, `#Machine Learning Infrastructure`

---

<a id="item-tech-news-10"></a>
### [AMD Launches Helion AI Rack System Supporting Up to 32,000 CPU Cores](https://news.google.com/rss/articles/CBMiU0FVX3lxTE5ybWpuSzh1Y2Z5X0djWUNvSFNnd0g4enlRXzhvVEpXZldnakhDVG9wdnlXTHd5aFQ0U2VXTDJxUUhSV1BwS01iblgzQy01NndoeHpR?oc=5) ⭐️ 8.0/10

AMD has introduced the Helion AI rack system, a scalable infrastructure solution designed to support up to 32,000 CPU cores. The system offers flexible configuration options, allowing data centers to deploy hybrid setups that combine pure CPU processing with GPU acceleration for AI workloads.

google\_news · 华尔街见闻 · Oct 12, 16:19

**「Background」** Modern AI infrastructure increasingly requires high-density, modular rack designs to manage the massive computational demands of large-scale model training and inference. This development follows the industry trend of integrating specialized hardware to optimize performance across diverse AI-driven tasks.

**「Impact」** Organizations can now scale their AI infrastructure more efficiently by utilizing the Helion system&\#x27;s high-density architecture, which reduces the physical footprint required for massive CPU-based compute clusters.

**Tags**: `#AMD`, `#Data Center`, `#AI Infrastructure`, `#Hardware`, `#High Performance Computing`

---

<a id="item-tech-news-11"></a>
### [Mistral AI Releases Le Chonk Model for Visual Grounding](https://aihot.news/items/s0j307n76znqj4xjmiapbjl7h) ⭐️ 7.0/10

Mistral AI has released a new model named Le Chonk, designed specifically for visual grounding tasks. The model achieves a 42% score on the Dense 200 benchmark, a performance metric that the company claims surpasses several existing frontier closed-source models.

rss · AIHOT 全站 · Oct 12, 16:49

**「Visual Grounding and the Dense200 Benchmark」** Visual grounding is a computer vision task that requires a model to precisely localize specific objects within complex, dense natural scenes rather than simply identifying them. The Dense200 benchmark is a specialized evaluation metric designed to measure the accuracy of these bounding-box localization capabilities.

**「Impact」** Developers working on computer vision applications requiring precise object localization may find Le Chonk to be a more capable alternative to current closed-source benchmarks, potentially improving accuracy in complex visual identification tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/dense200">Dense200 Leaderboard - llm-stats.com</a></li>

</ul>
</details>

**Tags**: `#Mistral AI`, `#Computer Vision`, `#Visual Grounding`, `#Artificial Intelligence`

---

<a id="item-tech-news-12"></a>
### [Allen Institute for AI releases open-weights AstaBrief model](https://allenai.org/blog/astabrief) ⭐️ 7.0/10

The Allen Institute for AI has released AstaBrief, an 8B parameter model specifically optimized for generating scientific reports with citations. The model is available as an open-weights release, providing researchers and developers with a specialized tool for document synthesis and retrieval-augmented generation tasks.

rss · Ai2 News · Oct 31, 00:00

**「Background」** Asta is a research initiative from the Allen Institute for AI focused on developing agentic tools to assist scientists with literature discovery and synthesis. These tools are designed to automate complex scholarly tasks, such as breaking down research queries and evaluating the relevance of scientific papers.

**「Impact」** Developers can now integrate AstaBrief into local or private pipelines to automate the creation of cited scientific summaries without relying on proprietary, closed-source model APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://allenai.org/asta">Asta: Advancing Scientific AI with Agents &amp; Benchmarks</a></li>
<li><a href="https://allenai.org/asta/agents">Asta Agents: AI Tools for Scientific Research</a></li>

</ul>
</details>

**Tags**: `#Artificial Intelligence`, `#Open Source`, `#Large Language Models`, `#Scientific Research`

---

<a id="item-tech-news-13"></a>
### [Yann LeCun Argues World Models, Not LLMs, Are Key to Future AI Breakthroughs](https://news.google.com/rss/articles/CBMiYkFVX3lxTFBtRndmN3ZjWjM1emdxRXQtYWRBbm1YSWw0MVJ3TFZBS0JnV0xIQ0RBb3dpNVpQUmVwemVWQkYxOWlCbFZpMklncjVIZ1ZIMzNBRFZMZ3A1U0JBYno4V1VxS2VB?oc=5) ⭐️ 7.0/10

Meta Chief AI Scientist Yann LeCun has stated that the next significant advancement in artificial intelligence will not emerge from scaling large language models \(LLMs\). Instead, he argues that the path to artificial general intelligence requires the development of &\#x27;world models&\#x27; capable of understanding physical reality and causal relationships. This perspective challenges the current industry reliance on transformer-based architectures for achieving human-level intelligence.

google\_news · 观点网 · Oct 12, 10:09

**「The Shift Toward World Models」** Yann LeCun has long maintained that current Large Language Models \(LLMs\) are fundamentally limited because they lack a physical understanding of the world, relying instead on statistical correlations in text. His proposed &\#x27;World Models&\#x27; architecture aims to enable AI systems to learn, predict, and reason about physical reality through observation and internal simulation, rather than just predicting the next token in a sequence.

**「Impact」** Researchers and organizations may need to shift focus from increasing parameter counts in LLMs toward developing architectures that can simulate physical environments and learn from observation, potentially altering long-term R&amp;D investment strategies.

**Tags**: `#Artificial Intelligence`, `#AGI`, `#Yann LeCun`, `#World Models`, `#Machine Learning`

---