---
layout: default
title: "Horizon Summary: 2026-10-23 (EN)"
date: 2026-10-23
lang: en
---

> From 107 items, 12 important content pieces were selected

---

**Technology News**
1. [Technical Analysis of Nintendo Switch 2 Jailbreak Methodology](#item-tech-news-1) ⭐️ 9.0/10
2. [Microsoft Introduces MAI-DxO AI Diagnostic System](#item-tech-news-2) ⭐️ 9.0/10
3. [Ai2&\#x27;s byte-level language model architecture Bolmo published in Nature](#item-tech-news-3) ⭐️ 9.0/10
4. [Oracle Issues Critical Security Alert for Java SE Vulnerability CVE-2026-91403](#item-tech-news-4) ⭐️ 9.0/10
5. [Quad9 to Cease DNS Operations in France Following Legal Pressure](#item-tech-news-5) ⭐️ 8.0/10
6. [NVIDIA Releases OpenShell for Secure Autonomous AI Agent Runtime](#item-tech-news-6) ⭐️ 8.0/10
7. [Microsoft and Hugging Face Release ThinkingBox-Training for RL Agent Development](#item-tech-news-7) ⭐️ 8.0/10
8. [Critical Vulnerability Surge Across Major Software Platforms](#item-tech-news-8) ⭐️ 8.0/10
9. [OpenAI 据报道正洽谈以 1.25 万亿美元估值融资至多 300 亿美元](#item-tech-news-9) ⭐️ 8.0/10
10. [Ai2 Releases Olmo-core 3 for Scalable Mixture-of-Experts Model Training](#item-tech-news-10) ⭐️ 8.0/10

**Technology Blog**
1. [Improving Agent Reliability via Database-Driven RL Rewards](#item-tech-blog-1) ⭐️ 9.0/10
2. [Ensemble Forecasting with IBM Granite Models](#item-tech-blog-2) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Technical Analysis of Nintendo Switch 2 Jailbreak Methodology](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) ⭐️ 9.0/10

Security researchers have detailed a jailbreak process for the Nintendo Switch 2, utilizing automated hardware interfaces to bypass console security. The methodology involves using JetKVMs for USB input and HDMI video capture, combined with physical automation tools like the SwitchBot Bot to manage power cycles during the exploitation process. This approach demonstrates a highly automated workflow for reverse-engineering and interacting with the console&\#x27;s firmware.

hackernews · ledoge · Oct 22, 08:01 · [Discussion](https://news.ycombinator.com/item?id=50192536)

**「Background」** The ns2jb exploit leverages a vulnerability within SmileBASIC 4, a programming environment originally released for the first-generation Nintendo Switch that remains compatible with the Switch 2. This software-based, tethered jailbreak allows users to execute arbitrary native code with the privileges of system modules, including the file system module, enabling homebrew execution and game modification.

**「Impact」** The successful implementation of read/write access to the console&\#x27;s file system could facilitate the rapid dumping of game software, potentially enabling the unauthorized execution of exclusive titles on non-Nintendo hardware.

**「Community Discussion」** Commenters expressed admiration for the sophisticated automation setup, noting that the integration of KVMs and physical actuators represents a significant advancement in hardware security research. Some users also debated the role of AI in assisting with such complex reverse-engineering tasks compared to traditional manual methods.

<details><summary>References</summary>
<ul>
<li><a href="https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/">pepsipu . com / blog / 2026 - 10 - switch 2 - jailbreak - ns 2 jb</a></li>
<li><a href="https://www.androidauthority.com/nintendo-switch-2-software-jailbreak-3727013/">Nintendo Switch 2 jailbreak could open the door to a world of mods</a></li>

</ul>
</details>

**Tags**: `#security`, `#hardware`, `#reverse-engineering`, `#gaming`, `#embedded-systems`

---

<a id="item-tech-news-2"></a>
### [Microsoft Introduces MAI-DxO AI Diagnostic System](https://aihot.news/items/ucpg7qczx7pzkl3eim00w7xgg) ⭐️ 9.0/10

Microsoft has unveiled MAI-DxO \(Microsoft AI Diagnostic Orchestrator\), an AI system that utilizes multi-agent orchestration to simulate collaborative medical consultations. The system manages the entire diagnostic process, including patient questioning, ordering examinations, and final assessment. According to research published in Science, the tool achieved an 83% accuracy rate on complex medical cases from the New England Journal of Medicine.

rss · AIHOT 全站 · Oct 22, 23:23

**「Background」** Medical diagnostic AI has historically struggled with complex clinical cases that require synthesizing diverse patient data and multi-step reasoning. Previous approaches often relied on single-model inference, which frequently failed to match the diagnostic accuracy of human specialists in challenging scenarios.

**「Impact」** The system&\#x27;s ability to outperform human diagnostic benchmarks in complex scenarios suggests a potential shift toward AI-assisted clinical decision-making, though its integration into real-world hospital workflows will require rigorous validation against diverse patient populations.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/the-path-to-medical-superintelligence/">The Path to Medical Superintelligence | Microsoft AI</a></li>
<li><a href="https://www.geekwire.com/2025/ai-vs-mds-microsoft-ai-tool-outperforms-doctors-in-diagnosing-complex-medical-cases/">AI vs. MDs: Microsoft tool hits 85.5% accuracy in tough diagnoses</a></li>

</ul>
</details>

**Tags**: `#Artificial Intelligence`, `#Healthcare AI`, `#Multi-Agent Systems`, `#Medical Diagnostics`, `#Microsoft`

---

<a id="item-tech-news-3"></a>
### [Ai2&\#x27;s byte-level language model architecture Bolmo published in Nature](https://allenai.org/blog/bolmo-nature) ⭐️ 9.0/10

The Allen Institute for AI \(Ai2\) has published its research on Bolmo, a language model architecture that operates directly on raw bytes rather than traditional subword tokens, in the journal Nature. By eliminating the tokenization layer, this approach aims to improve model performance across diverse languages and domains that are often poorly represented by standard tokenizers.

rss · Ai2 News · Oct 31, 00:00

**「Background」** Standard language models typically rely on subword tokenization, which can introduce limitations in handling multilingual text and non-standard character sets. Bolmo addresses this by using a two-stage conversion process to adapt existing subword-based models, such as OLMo, into byte-level architectures that operate directly on raw bytes.

**「Impact」** Developers and researchers can now utilize Bolmo&\#x27;s byte-level architecture to bypass common tokenization bottlenecks, potentially reducing bias and improving accuracy in multilingual applications or tasks involving non-standard text formats.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2512.15586">Bolmo : Byteifying the Next Generation of Language Models</a></li>
<li><a href="https://allenai.org/blog/bolmo">Introducing Bolmo : Byteifying the next generation of language models</a></li>

</ul>
</details>

**Tags**: `#Artificial Intelligence`, `#Language Models`, `#Machine Learning`, `#Open Source`, `#Research`

---

<a id="item-tech-news-4"></a>
### [Oracle Issues Critical Security Alert for Java SE Vulnerability CVE-2026-91403](https://www.oracle.com/security-alerts/alert-cve-2026-91403.html) ⭐️ 9.0/10

Oracle has identified a critical vulnerability, CVE-2026-91403, in the JSSE component of Java SE and GraalVM with a CVSS score of 9.1. The flaw allows unauthenticated remote attackers to compromise data confidentiality and integrity, affecting versions including Java SE 8u511, 11.0.33, 17.0.21, 21.0.13, 25.0.5, and 27.0.1. Oracle has released patches and urges users to update to the latest supported versions immediately to mitigate exploitation risks.

telegram · zaihuapd · Oct 22, 12:30

**「Background」** The Java Secure Socket Extension \(JSSE\) is a core component of the Java platform that enables secure internet communications by implementing SSL and TLS protocols. Vulnerabilities in this component are particularly severe because they can expose encrypted traffic or bypass authentication mechanisms in enterprise applications.

**「Impact」** System administrators and developers must prioritize patching their Java environments, as the vulnerability&\#x27;s high CVSS score and lack of required authentication make it a prime target for automated remote exploitation.

**Tags**: `#Java`, `#Cybersecurity`, `#Vulnerability`, `#Oracle`, `#Software Engineering`

---

<a id="item-tech-news-5"></a>
### [Quad9 to Cease DNS Operations in France Following Legal Pressure](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 8.0/10

Quad9 is withdrawing its DNS resolution services from France, with a planned service termination date of November 24. The decision follows ongoing legal pressure and court-imposed fines related to mandatory website blocking orders, which the organization argues are technically incompatible with its operational model. Quad9 intends to implement GeoIP filtering to restrict access for users located within France.

hackernews · farrokhi · Oct 22, 14:32 · [Discussion](https://news.ycombinator.com/item?id=50195959)

**「Legal Context of DNS Blocking in France」** French media companies, including Canal+ and beIN Sports, have increasingly utilized court-ordered injunctions to force DNS resolvers to block access to websites accused of copyright infringement. As reported by Horizon&\#x27;s December 10, 2024 digest, Quad9 faced initial legal pressure from Canal+ shortly after resolving a similar copyright-related case in Germany, eventually leading to the current decision to cease operations in France to avoid further penalties for non-compliance.

**「Operational Consequences for French Users」** French users relying on Quad9 for DNS resolution must transition to alternative providers by November 24, as the service will implement GeoIP filtering to block access from France to comply with legal mandates. This withdrawal follows a pattern of French courts compelling DNS operators to enforce site-blocking injunctions, a requirement that previously forced Cisco to exit the market and compelled Google and Cloudflare to implement similar restrictions.

**「Community Discussion」** Commenters expressed frustration over the legal precedent of holding DNS resolvers liable for content access, comparing it to penalizing a phone book provider for the actions of listed individuals. Users also noted that this exit mirrors previous actions taken by other infrastructure providers facing similar injunctions from French media entities regarding sports piracy.

<details><summary>References</summary>
<ul>
<li><a href="https://quad9.net/news/press/quad9-faces-new-dns-censorship-legal-challenge-in-france-from-canal/">Quad9 Faces New DNS Censorship Legal Challenge in France from ...</a></li>
<li><a href="https://reclaimthenet.org/quad9-considers-leaving-france-over-website-blocking-order">Quad9 Considers Leaving France Over Website Blocking Order</a></li>
<li><a href="https://torrentfreak.com/dns-block-canal-sues-cloudflare-google-cisco-to-fight-piracy-231230/">DNS Block : Canal+ Sues Cloudflare, Google &amp; Cisco ... * TorrentFreak</a></li>
<li><a href="https://www.torlock.com/news/11381/court-upholds-belgian-pirate-dns-blocking-order-opendns-exit-looms.html">Court Upholds Belgian Pirate DNS Blocking Order, OpenDNS Exit ...</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#Internet Censorship`, `#Privacy`, `#Legal`, `#Infrastructure`

---

<a id="item-tech-news-6"></a>
### [NVIDIA Releases OpenShell for Secure Autonomous AI Agent Runtime](https://github.com/NVIDIA/OpenShell) ⭐️ 8.0/10

NVIDIA has released OpenShell, a runtime environment designed to manage autonomous AI agents by enforcing security policies through containerization. The tool restricts agent access to local files, network resources, and credentials, providing a controlled sandbox for agents that require system-level capabilities. It aims to mitigate risks such as unauthorized data exfiltration and credential misuse while maintaining agent functionality.

hackernews · niemandhier · Oct 22, 17:44 · [Discussion](https://news.ycombinator.com/item?id=50198675)

**「Context for AI Agent Security」** Autonomous AI agents require broad system permissions—such as file system access, network connectivity, and credential usage—to perform complex tasks, which creates significant security risks regarding data exfiltration and unauthorized system modification. OpenShell addresses these challenges by implementing a policy-driven runtime that treats agent workloads as untrusted, enforcing granular access controls through containerization and governance frameworks.

**「Impact」** Developers can now implement granular security boundaries for AI agents, reducing the risk of malicious or unintended actions by limiting agent access to specific system resources and network domains.

**「Community Discussion」** Users generally welcome the containerized approach to agent security, though some express skepticism about whether any runtime can fully resolve the inherent tension between granting agents high-level capabilities and maintaining strict data isolation. Others noted that while OpenShell provides a solid foundation, additional layers for policy management and security scanning are often required for production-grade deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/ai/openshell/">NVIDIA OpenShell | Open, Secure Runtime for AI Agents</a></li>
<li><a href="https://github.com/NVIDIA/OpenShell">OpenShell – private runtime for autonomous AI agents</a></li>
<li><a href="https://developer.nvidia.com/blog/how-nvidia-openshell-reference-architecture-secures-and-governs-ai-agent-workloads-at-scale/">How NVIDIA OpenShell Reference Architecture Secures and ...</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Security`, `#Containerization`, `#NVIDIA`, `#Software Engineering`

---

<a id="item-tech-news-7"></a>
### [Microsoft and Hugging Face Release ThinkingBox-Training for RL Agent Development](https://aihot.news/items/c1wb4w4ehhq5ig4m4hwv3kbbp) ⭐️ 8.0/10

Microsoft and Hugging Face have released ThinkingBox-Training, an open-source framework designed to improve AI agent performance through reinforcement learning. The system utilizes the execution results of database queries as objective reward signals to evaluate and train agents on complex tasks. The code is currently available on GitHub for developers to integrate into their agentic training workflows.

rss · AIHOT 全站 · Oct 22, 22:24

**「Background」** ThinkingBox was introduced in early October 2026 as a benchmark and sandbox environment containing 507 stateful business workflows designed to evaluate AI agents based on terminal database states and side effects. The framework addresses the reliability gap in agentic systems by verifying task completion through actual backend execution rather than relying solely on an agent&\#x27;s self-reported success.

**「Impact」** Developers can now use verifiable database outcomes as a reliable feedback mechanism for reinforcement learning, reducing reliance on subjective or less precise reward models when training agents to perform data-driven tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://riverfrontai.com/journal/microsoft-s-thinkingbox-grades-ai-agents-on-database-state-n-3ef2c1b9">Microsoft&#x27;s ThinkingBox Grades AI Agents on Database State ...</a></li>
<li><a href="https://huggingface.co/blog/microsoft/thinkingbox">The Agent Said It Was Done. The Database Disagreed.</a></li>

</ul>
</details>

**Tags**: `#Reinforcement Learning`, `#AI Agents`, `#Microsoft`, `#Hugging Face`, `#Machine Learning`

---

<a id="item-tech-news-8"></a>
### [Critical Vulnerability Surge Across Major Software Platforms](https://aihot.news/items/bw9sz0kx1l5ousd589zo3ficm) ⭐️ 8.0/10

Multiple critical security vulnerabilities were disclosed within a 48-hour period, affecting major infrastructure including PHP, GitLab, Node.js, Chrome, Oracle, and Atlassian. Notable reports include a CVSS 10.0 remote code execution \(RCE\) vulnerability in GitLab, an unauthenticated RCE in PHP, and an RCE in the Node.js Brotli decoder. Additionally, vendors have released massive security updates, such as 1,295 patches for Oracle and 353 fixes for Chrome.

rss · AIHOT 全站 · Oct 22, 22:21

**「Vulnerability Context」** These disclosures follow the recent identification of critical remote code execution \(RCE\) flaws in PHP \(CVE-2026-109618 and CVE-2026-109619\) and GitLab \(CVE-2026-110264\), which allow unauthenticated attackers to compromise affected systems. Such vulnerabilities are typically addressed through vendor-issued security patches that require immediate deployment to mitigate the risk of unauthorized system access.

**「Impact」** Organizations and developers must prioritize immediate patching and security audits of their environments, as these vulnerabilities allow for remote code execution across core development and production infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/10/critical-gitlab-flaw-cvss-100-could.html?m=1">Critical GitLab Flaw (CVSS 10.0) Could Allow Unauthenticated RCE...</a></li>
<li><a href="https://ubuntu.com/blog/php2shell-vulnerability-fixes-available">php 2shell (CVE- 2026 -109618 and CVE- 2026 -109619) – PHP critical ...</a></li>
<li><a href="https://www.digitalocean.com/blog/critical-php-rce-vulnerabilities-patch-now">Critical PHP RCE Vulnerabilities : Patch Now (CVE- 2026 -109618...)</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#vulnerability`, `#software-engineering`, `#infrastructure`, `#devops`

---

<a id="item-tech-news-9"></a>
### [OpenAI 据报道正洽谈以 1.25 万亿美元估值融资至多 300 亿美元](https://aihot.news/items/wg3g8yf3e8c11smv9q88k4poz) ⭐️ 8.0/10

OpenAI is reportedly in talks to raise up to $30 billion at a $1.25 trillion valuation, with potential strategic partnerships involving compute resources.

rss · AIHOT 全站 · Oct 22, 22:08

**Tags**: `#OpenAI`, `#AI Industry`, `#Venture Capital`, `#Artificial Intelligence`, `#Corporate Strategy`

---

<a id="item-tech-news-10"></a>
### [Ai2 Releases Olmo-core 3 for Scalable Mixture-of-Experts Model Training](https://allenai.org/blog/olmocore3) ⭐️ 8.0/10

The Allen Institute for AI \(Ai2\) has released Olmo-core 3, an open-source training infrastructure specifically engineered to improve the efficiency and scalability of Mixture-of-Experts \(MoE\) language models. This redesigned stack provides researchers with the tools necessary to train large-scale MoE architectures, aiming to increase transparency and accessibility in high-performance model development.

rss · Ai2 News · Oct 31, 00:00

**「Background」** Mixture-of-Experts \(MoE\) architectures improve model efficiency by activating only a subset of parameters for each input, but they introduce significant complexity in distributed training and load balancing. Previous training stacks often relied on proprietary or opaque implementations, limiting the ability of researchers to optimize communication patterns and expert routing at scale.

**「Performance and Scalability Gains」** Researchers and developers can achieve a 2.7x increase in training throughput compared to previous iterations by utilizing Olmo-core 3&\#x27;s optimized routing mechanism, which directs data to resident experts rather than relying on repeated weight gathering. This infrastructure enables the training of models reaching the trillion-parameter scale, though users should note that certain experimental features like weight offloading may negatively impact training speed.

<details><summary>References</summary>
<ul>
<li><a href="https://allenai.org/blog/olmocore3">Introducing Olmo-core 3: Open, scalable training ...</a></li>
<li><a href="https://www.unite.ai/ai2-releases-olmo-core-3-open-training-stack-for-trillion-parameter-moes/">Ai2 Releases Olmo-Core 3, Open Training Stack for Trillion ...</a></li>
<li><a href="https://www.techtimes.com/articles/328470/20261002/ai2-releases-olmocore-3-open-moe-training-stack-delivers-27x-throughput-gain.htm">Ai2 Releases OlmoCore 3: Open MoE Training Stack Delivers 2 ...</a></li>

</ul>
</details>

**Tags**: `#Artificial Intelligence`, `#Machine Learning`, `#Open Source`, `#Large Language Models`, `#Distributed Systems`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Improving Agent Reliability via Database-Driven RL Rewards](https://huggingface.co/blog/microsoft/thinkingbox-training) ⭐️ 9.0/10

rss · Hugging Face Blog · Oct 22, 22:24

**「背景」** Agentic workflows often suffer from a &\#x27;dependability gap,&\#x27; where models may solve a task once but fail to do so consistently, leading to unreliable outcomes in production database environments. The authors argue that standard headline accuracy metrics fail to capture this inconsistency, necessitating a more rigorous approach to evaluating and training agents that interact with real backend states.

**「方案」** The authors introduce ThinkingBox-Training, a framework that treats executable database terminal states as direct reinforcement learning \(RL\) rewards. To maximize the effectiveness of Group Relative Policy Optimization \(GRPO\), they implement &\#x27;offline policy-relative difficulty&\#x27; filtering, which selects training tasks that are neither too easy nor too hard for the base model, ensuring the agent receives meaningful contrastive feedback. By fine-tuning a Qwen3.8-27B model on 187 curated tasks, the authors observed a significant increase in repeatable success—tasks completed correctly across all 20 attempts rose from 7.5% to 21.1%. The process emphasizes strict parity between training and evaluation parsers to ensure that the reward signal accurately reflects the agent&\#x27;s actual performance on production-like database records.

**「启示」** Reliability in agentic systems is best achieved by shifting from simple success metrics to measuring repeatable performance, using executable database states as the primary reward signal. This approach demonstrates that agents can be sharpened for production consistency by training on tasks specifically selected for their potential to provide contrastive learning signals.

**Tags**: `#Reinforcement Learning`, `#Agentic Workflows`, `#Model Evaluation`, `#Database Reliability`, `#GRPO`

---

<a id="item-tech-blog-2"></a>
### [Ensemble Forecasting with IBM Granite Models](https://huggingface.co/blog/ibm-research/granite-timeseries-ensemble-r1) ⭐️ 8.0/10

rss · Hugging Face Blog · Oct 22, 07:51

**「Background」** Selecting the optimal pre-trained time-series model is often difficult because different architectures—such as Transformers, state-space models, or MLP mixers—excel at different types of data, from smooth industrial signals to noisy retail demand. Relying on a single model risks poor performance if the chosen architecture is ill-suited to the specific characteristics of the target dataset.

**「Solution」** The Granite Timeseries Ensemble addresses this by combining four distinct Granite architectures into a single, extensible interface that requires no retraining or weight optimization. The framework offers two primary aggregation recipes: a Probabilistic Ensemble that pools quantile forecasts with equal influence, and an IQR Ensemble that adaptively weights members based on their forecast spread. By merging these complementary views, the ensemble provides a robust, unified forecast that consistently outperforms individual members on aggregate metrics like MASE in the GIFT-Eval benchmark. While this approach increases inference latency and memory overhead due to loading multiple checkpoints, it provides a reliable default that avoids the need for manual model selection. Practitioners can further customize the ensemble by swapping in external models or adjusting the aggregation logic, provided they account for the increased computational costs and verify performance on their specific domain data.

**「Takeaway」** Ensemble forecasting with Granite models provides a robust, low-effort default that delivers consistent performance across diverse datasets by mitigating the risks of choosing a single, potentially mismatched architecture. It shifts the focus from model selection to a scalable, unified interface that balances accuracy with operational simplicity.

**Tags**: `#time-series-forecasting`, `#ensemble-learning`, `#machine-learning-engineering`, `#probabilistic-forecasting`

---