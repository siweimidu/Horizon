---
layout: default
title: "Horizon Summary: 2026-10-17 (ZH)"
date: 2026-10-17
lang: zh
---

> 从 100 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Claude 揭示 NIST 椭圆曲线种子生成机制](#item-tech-news-1) ⭐️ 9.0/10
2. [Meta 发布 Muse Spark Open：816B 参数 MoE 模型及 1M 上下文支持](#item-tech-news-2) ⭐️ 9.0/10
3. [艾伦人工智能研究所 \(Ai2\) 的字节级语言模型 Bolmo 研究发表于《自然》](#item-tech-news-3) ⭐️ 9.0/10
4. [研究人员推出 ORL 与 dlmrt 引擎，大幅提升扩散语言模型推理速度](#item-tech-news-4) ⭐️ 9.0/10
5. [Black Forest Labs 发布 FLUX 3 图像生成模型](#item-tech-news-5) ⭐️ 8.0/10
6. [Unsloth 适配 NVIDIA RTX Spark，支持笔记本本地训练 120B+ 参数模型](#item-tech-news-6) ⭐️ 8.0/10
7. [Anthropic 报告：AI 智能体工作时长达人类 6 倍，初级岗位招聘缩减](#item-tech-news-7) ⭐️ 8.0/10
8. [Anthropic 向美国国会提交 AI 监管草案，设定干预门槛](#item-tech-news-8) ⭐️ 8.0/10
9. [DeepSeek 开源 TileLang 升腾后端以支持跨平台 AI 计算](#item-tech-news-9) ⭐️ 8.0/10
10. [Anthropic 研究显示 Claude 可自主设计更高效的量子电路](#item-tech-news-10) ⭐️ 8.0/10
11. [Ai2 发布 Olmo-core 3：用于大规模 MoE 模型训练的开源基础设施](#item-tech-news-11) ⭐️ 8.0/10

**科技博客**
1. [构建大规模印度语言预训练数据集与开源生成流水线](#item-tech-blog-1) ⭐️ 9.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude 揭示 NIST 椭圆曲线种子生成机制](https://www.anthropic.com/research/ecdsa-curve-origins) ⭐️ 9.0/10

研究人员利用 Claude 模型成功破解了 NIST P 系列椭圆曲线（P-192、P-224、P-256、P-384 和 P-521）的种子生成方式。分析显示，这些种子并非源自复杂的哈希算法，而是通过 C 语言库中的 lrand48 随机数生成器，并以 Unix 时间戳作为种子生成的。除 B-163 曲线外，其余所有 NIST P 系列曲线的种子来源均已得到确认。

hackernews · Anthropic Research · 10月16日 18:55 · [社区讨论](https://news.ycombinator.com/item?id=50122800)

**「背景」** NIST 椭圆曲线的种子生成方式长期以来因缺乏透明度而备受质疑，外界曾广泛猜测其可能存在预留的后门或恶意设计。这一发现为持续数十年的密码学阴谋论提供了明确的解释。

**「影响」** 该研究通过证实 NIST 曲线种子生成过程的简单性，有效消除了关于这些广泛使用的加密标准中存在恶意后门的长期担忧，从而增强了业界对现有椭圆曲线密码标准的信任。

**「社区讨论」** 社区成员普遍认为这一发现是对多年阴谋论的有力反驳，但也指出该结果仅解释了生成方法，无法完全排除在生成过程中通过筛选特定时间戳来挑选曲线属性的可能性。此外，有评论推测 B-163 曲线无法匹配的原因可能是发布时的录入错误。

**标签**: `#cryptography`, `#nist`, `#security`, `#ai-research`, `#elliptic-curves`

---

<a id="item-tech-news-2"></a>
### [Meta 发布 Muse Spark Open：816B 参数 MoE 模型及 1M 上下文支持](https://aihot.news/items/ueqic1dy2hdx4ua7yipobons6) ⭐️ 9.0/10

Meta 正式发布了 Muse Spark Open，这是一款拥有 816B 参数的开源权重混合专家（MoE）模型，并支持高达 1M 的上下文窗口。该模型旨在为开发者提供高性能的开源 AI 选项，使其具备处理超长文本序列的能力。

rss · AIHOT 全站 · 10月17日 00:06

**「背景信息」** 混合专家模型（MoE）通过仅激活总参数中的一小部分来处理每个 token，从而在保持大规模模型知识容量的同时降低推理计算成本。Muse Spark Open 采用这种架构，通过 42B 的活跃参数支持 1M token 的长上下文处理，旨在提升长周期代理任务（如复杂编程和客户服务）的执行能力。

**「影响」** Muse Spark Open 的发布显著提升了开源社区处理大规模上下文任务的上限，使得开发者能够在本地或私有环境中部署具备超长记忆能力的复杂推理模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/meta-muse-spark-open-816b-open-weight-agentic-coding-model-how-to-run-2026">Muse Spark Open: Meta 816B Open Model, How to Run It ...</a></li>
<li><a href="https://dev.meta.ai/resources/blog/build-with-muse-spark-open">Build with Muse Spark Open - dev.meta.ai</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Large Language Models`, `#MoE`, `#Open Source AI`, `#Meta`

---

<a id="item-tech-news-3"></a>
### [艾伦人工智能研究所 \(Ai2\) 的字节级语言模型 Bolmo 研究发表于《自然》](https://allenai.org/blog/bolmo-nature) ⭐️ 9.0/10

艾伦人工智能研究所 \(Ai2\) 开发的字节级语言模型 Bolmo 的相关研究已正式发表于《自然》期刊。该模型摒弃了传统的标记化 \(tokenization\) 处理方式，直接在字节层面进行操作，旨在解决现有语言模型在多语言和跨领域任务中的基础性局限。

rss · Ai2 News · 10月31日 00:00

**「背景」** 传统大语言模型通常依赖分词器（Tokenization）将文本转换为子词单元，这在处理多语言或跨领域任务时常受限于词表覆盖范围。Bolmo 架构通过“字节化”（Byteification）技术，允许模型直接在字节级别进行处理，从而绕过了分词器的限制。该方法最初于 2025 年 12 月作为开源项目发布，旨在通过两阶段转换流程，使现有模型在无需大量额外训练的情况下具备字节级处理能力。

**「影响」** 通过绕过标记化过程，Bolmo 为开发者提供了一种更具通用性的架构，能够有效提升模型在处理非标准文本、多语言数据及复杂字符集时的性能与鲁棒性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41586-026-11111-4">Retrofitting language models to operate over bytes | Nature</a></li>
<li><a href="https://arxiv.org/abs/2512.15586">[2512.15586] Bolmo: Byteifying the Next Generation of ... Bolmo: Byteifying the Next Generation of Language Models Retrofitting language models to operate over bytes Introducing Bolmo: Byteifying the next generation of language ... Now in Nature: Retrofitting language models to operate over ... Now in Nature: Retrofitting language models to operate over…</a></li>
<li><a href="https://arxiv.org/pdf/2512.15586">Bolmo: Byteifying the Next Generation of Language Models</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Language Models`, `#Machine Learning`, `#Research`, `#Open Source`

---

<a id="item-tech-news-4"></a>
### [研究人员推出 ORL 与 dlmrt 引擎，大幅提升扩散语言模型推理速度](https://www.reddit.com/r/MachineLearning/comments/1x7qgr0/research_2788_tokenss_on_a_single_rtx_5090_with_a/) ⭐️ 9.0/10

研究人员发布了“在线残差学习”（ORL）训练方法及配套的 dlmrt 推理引擎，旨在提升扩散语言模型（dLLM）的生成效率。在单张 RTX 5090 显卡上，使用 LLaDA-2.1-mini 模型配合 NVFP4 量化，推理速度可达 2,788 tokens/s。该方案通过在推理过程中直接利用模型生成的残差状态进行训练，并结合 CUDA 图优化，实现了比传统自回归模型及现有推测解码方案更高的端到端吞吐量。

reddit · r/MachineLearning · /u/arty\_photography · 10月16日 20:03

**「背景信息」** 传统的自回归大语言模型（LLM）通常逐个生成 token，而扩散语言模型通过并行细化多个 token 来生成文本。ORL 通过引入“相邻熵收缩”机制，使模型在每个去噪步骤中能更有效地减少不确定性，从而在保持生成质量的同时减少所需的推理步数。

**「影响与应用」** 开发者和研究人员现在可以利用开源的 ORL 训练代码和 dlmrt 引擎，在消费级硬件（如 RTX 5090）上实现极高吞吐量的单请求推理。对于需要低延迟生成任务的应用场景，该技术提供了一种替代传统自回归推理的有效路径。

**标签**: `#Machine Learning`, `#Diffusion Models`, `#Inference Optimization`, `#LLM`, `#Open Source`

---

<a id="item-tech-news-5"></a>
### [Black Forest Labs 发布 FLUX 3 图像生成模型](https://bfl.ai/blog/flux-3-image-klein) ⭐️ 8.0/10

Black Forest Labs 发布了 FLUX 3 图像生成模型，该模型以紧凑的架构（小于 10GB）和极具竞争力的定价（起价为每 1000 张图像 0.009 美元）为主要卖点。尽管该模型在图像编辑能力上表现稳健，但用户反馈指出其在处理精细文本细节方面存在局限，且部分用户报告了生成人体图像时出现异常输出的问题。

hackernews · gmays · 10月16日 19:47 · [社区讨论](https://news.ycombinator.com/item?id=50123580)

**「背景信息」** FLUX 3 Image Klein 是 Black Forest Labs 推出的最新开源权重图像生成模型，该模型整合了该公司在图像、视频和音频多模态学习方面的技术积累。此前，Black Forest Labs 强调了其在模型开发中对安全性的评估，特别是在防范非法内容生成方面的风险缓解措施。

**「市场竞争与成本影响」** FLUX 3 以每 1000 张图像 0.009 美元的定价进入市场，显著低于近期发布的 Krea 3（约 0.06 美元/张）等竞品，为追求高性价比的大规模图像生成任务提供了更具成本优势的选择。开发者在选择模型时需权衡 FLUX 3 在文本渲染和人体结构生成方面的潜在局限性，与 Krea 3 针对生产环境优化的区域编辑能力进行对比评估。

**「社区讨论」** 社区成员讨论了 FLUX 3 与近期发布的 Krea 3 等竞品在价格和质量上的差异，并质疑其对人体图像生成能力的限制是否源于训练数据中移除了 NSFW 内容。此外，部分用户认为该模型在处理复杂细节时表现不佳，并将其与近期发布的其他模型进行了对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bfl.ai/blog/flux-3-image-klein">FLUX 3 Image Klein : open weights, 5.6B parameters | Black Forest ...</a></li>
<li><a href="https://comfy.org/flux-3-image-klein/">FLUX 3 Image Klein Launch | Comfy</a></li>
<li><a href="https://huggingface.co/black-forest-labs/flux-3-image-klein">black - forest - labs / flux - 3 - image - klein · Hugging Face</a></li>
<li><a href="https://www.krea.ai/krea-3">Krea 3 : an image model built for editing at scale</a></li>
<li><a href="https://news.ycombinator.com/item?id=50105648">Krea 3 – An image model built for editing at scale | Hacker News</a></li>

</ul>
</details>

**标签**: `#generative-ai`, `#image-synthesis`, `#machine-learning`, `#model-efficiency`

---

<a id="item-tech-news-6"></a>
### [Unsloth 适配 NVIDIA RTX Spark，支持笔记本本地训练 120B+ 参数模型](https://aihot.news/items/gfh55ke3d2q7ikzu9vzyve289) ⭐️ 8.0/10

Unsloth 现已适配 NVIDIA RTX Spark 平台，支持在笔记本电脑上本地运行并微调 120B+ 参数规模的模型。通过针对 ARM 架构优化的 CUDA 内核与二进制文件，该方案在训练扩散、决策及多模态模型时的速度较此前提升约 2.7 倍，并支持最高 128GB 的统一内存配置。

rss · AIHOT 全站 · 10月16日 23:54

**「背景信息」** NVIDIA RTX Spark 是 NVIDIA 推出的首款针对 Windows on ARM 平台的笔记本超级芯片，旨在通过集成 AI 加速能力提升轻薄设备的本地计算性能。该平台支持统一内存架构，为在移动设备上运行和微调大规模参数模型提供了硬件基础。

**「实际影响」** 该适配显著降低了超大规模模型微调的硬件门槛，使得开发者无需依赖云端算力，即可在消费级笔记本硬件上完成 120B+ 参数模型的本地训练任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/products/rtx-spark/">Slim Laptops &amp; Small Desktops | NVIDIA RTX Spark</a></li>
<li><a href="https://www.youtube.com/watch?v=9tq71nn0u0c">Nvidia &#x27;s RTX Spark Is Here: The Future of Windows Laptops ?</a></li>
<li><a href="https://www.tomshardware.com/laptops/we-test-the-rtx-spark-superchip-in-microsofts-surface-laptop-ultra-nvidias-windows-on-arm-platform-impresses-in-local-ai-but-gaming-isnt-its-strong-suit">We test the RTX Spark Superchip in Microsoft&#x27;s Surface Laptop Ultra...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Fine-tuning`, `#NVIDIA`, `#Hardware Acceleration`, `#Unsloth`

---

<a id="item-tech-news-7"></a>
### [Anthropic 报告：AI 智能体工作时长达人类 6 倍，初级岗位招聘缩减](https://aihot.news/items/we5x0aeailoezuugv834oxpr2) ⭐️ 8.0/10

Anthropic 发布报告显示，截至 2026 年 8 月，其内部部署的交互式 AI 智能体工作时长已达到人类员工的 6 倍。该效率提升伴随着显著的经济产出增长，其人均创收达到 Meta 和谷歌同期的 2 至 4 倍。

rss · AIHOT 全站 · 10月16日 23:13

**「背景信息」** Anthropic 此前已在内部实践中逐步增加 AI 智能体在技术工作流中的应用，并观察到初级技术岗位的招聘比例随之下降。这一趋势反映了企业在提升自动化生产力过程中，对传统入门级人力需求结构的调整。

**「影响分析」** AI 智能体的高效产出直接改变了企业的人才需求结构，导致初级技术岗位的招聘占比从 27% 大幅下降至 9%，表明企业正通过自动化手段替代部分入门级人力资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/employment-at-anthropic">How employment is changing at Anthropic \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Labor Market`, `#Productivity`, `#Anthropic`, `#Industry Trends`

---

<a id="item-tech-news-8"></a>
### [Anthropic 向美国国会提交 AI 监管草案，设定干预门槛](https://aihot.news/items/jxszzjrwfc4656n0m8oh0elgt) ⭐️ 8.0/10

Anthropic 已向美国国会议员提交一份 AI 安全与防务监管法案草案，旨在明确政府叫停 AI 模型的具体触发条件。根据草案，政府仅在模型可预见地导致超过 10 亿美元经济损失，或造成 50 人以上死亡或重伤，且风险源于生物武器、模型失控或严重网络攻击时，方可采取叫停措施。

rss · AIHOT 全站 · 10月16日 23:05

**「背景信息」** Anthropic 作为一家专注于 AI 安全与可解释性的研究公司，此前已多次参与 AI 监管政策的讨论，并曾通过其政府关系部门推动针对前沿 AI 系统的立法进程。此次草案中引用的加州 SB 53 等法案，是近年来美国各州为应对 AI 快速发展而尝试建立的监管框架，旨在平衡技术创新与公共安全风险。

**「影响」** 该草案若被采纳，将为 AI 监管设定明确的量化门槛，从而在法律层面限制政府对 AI 研发的行政干预范围，为企业提供更清晰的合规预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research">Research \ Anthropic</a></li>
<li><a href="https://www.trymurph.com/insights/anthropic-s-state-ai-lobbying-looks-less-like-safety-more-like-moat">Anthropic &#x27;s State AI Lobbying Looks Less Like Safety , More Like Moat</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#AI Safety`, `#Regulation`, `#Anthropic`, `#Governance`

---

<a id="item-tech-news-9"></a>
### [DeepSeek 开源 TileLang 升腾后端以支持跨平台 AI 计算](https://aihot.news/items/hbvfpex76ecwu9amvds2er8o0) ⭐️ 8.0/10

DeepSeek 于 9 月 30 日开源了面向华为升腾（Ascend）平台的编程基础设施，包括计算与通信库。此次更新在 TileKernels 仓库中新增了升腾后端，使开发者能够通过统一的 Python API 在 Nvidia GPU 和华为 NPU 上运行相同的代码。

rss · AIHOT 全站 · 10月16日 22:39

**「背景」** TileLang 是 DeepSeek 开发的一种编程框架，旨在通过抽象底层硬件差异来简化高性能算子的编写。此前该框架主要针对 Nvidia GPU 架构，此次扩展旨在解决 AI 训练和推理过程中对单一硬件供应商的依赖问题。

**「影响」** 该举措降低了 AI 模型在不同硬件平台间迁移的开发成本，使企业和开发者能够更灵活地在华为升腾 NPU 上部署模型，从而减少对 Nvidia 硬件生态的依赖。

**标签**: `#DeepSeek`, `#Huawei Ascend`, `#AI Infrastructure`, `#Open Source`, `#Hardware Abstraction`

---

<a id="item-tech-news-10"></a>
### [Anthropic 研究显示 Claude 可自主设计更高效的量子电路](https://www.anthropic.com/research/designing-efficient-quantum-circuits) ⭐️ 8.0/10

Anthropic 研究人员通过向 Claude 提供八种量子电路的自然语言规范及自动化评估工具，成功使其自主设计出性能优于现有已发表基准的电路。在部分案例中，Claude 设计的电路效率提升了一个数量级或更多，展示了大型语言模型在硬件优化领域的潜力。

rss · Anthropic Research · 10月16日 17:29

**「背景」** 量子电路设计通常依赖于复杂的人工优化，旨在减少门操作数量以降低量子计算过程中的退相干误差。此前，该领域主要依靠人类专家或专门的启发式算法进行电路架构的迭代。

**「影响」** 该研究表明 AI 辅助设计有望显著降低量子计算的硬件门控开销，从而加速实用化量子计算机的研发进程，并为复杂量子算法的实现提供更高效的底层架构支持。

**标签**: `#Quantum Computing`, `#Artificial Intelligence`, `#Hardware Design`, `#Research`

---

<a id="item-tech-news-11"></a>
### [Ai2 发布 Olmo-core 3：用于大规模 MoE 模型训练的开源基础设施](https://allenai.org/blog/olmocore3) ⭐️ 8.0/10

艾伦人工智能研究所（Ai2）发布了 Olmo-core 3，这是一套专为混合专家模型（MoE）设计的开源训练基础设施。该系统通过重新设计的架构，旨在解决大规模 MoE 模型在训练过程中的效率瓶颈，并提升分布式训练的扩展性。

rss · Ai2 News · 10月31日 00:00

**「背景信息」** 混合专家模型（MoE）通过仅激活模型参数的一小部分来处理每个输入，从而在保持高性能的同时降低了计算成本。然而，由于其复杂的稀疏架构，在分布式计算环境中高效训练此类模型一直面临着通信开销和负载均衡等技术挑战。

**「对开发者的影响」** 研究人员和开发者现在可以利用 Olmo-core 3 的分布式训练技术，在 GPU 集群上更高效地分配和训练参数规模达到万亿级别的混合专家（MoE）模型，从而降低大规模模型训练中的路由与计算瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allenai.org/blog/olmocore3">Introducing Olmo - core 3 : Open, scalable training infrastructure for...</a></li>
<li><a href="https://huggingface.co/blog/allenai/olmocore3">Introducing Olmo - core 3 : Open, scalable training infrastructure for...</a></li>
<li><a href="https://daily.dev/posts/introducing-olmo-core-3-open-scalable-training-infrastructure-for-large-moes-vzgcmhplj">Introducing Olmo - core 3 : Open, scalable training ...</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Machine Learning`, `#Open Source`, `#Distributed Systems`, `#MoE`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [构建大规模印度语言预训练数据集与开源生成流水线](https://huggingface.co/blog/nvidia/scaling-indic-pretraining) ⭐️ 9.0/10

rss · Hugging Face Blog · 10月16日 01:44

**「背景」** 印度语言模型的发展长期受限于高质量训练数据的匮乏，导致其在技术理解与推理能力上显著落后于英语模型。为了弥补这一差距，NVIDIA 与印度理工学院马德拉斯分校（IIT Madras）的 AI4Bharat 实验室合作，旨在通过大规模合成数据生成来扩充印度语言的预训练语料库。

**「方案」** 该项目构建了一个包含 2.8 万亿 Token 的印度语言数据集，涵盖 22 种宪法认可的语言及 34 种语言-脚本配置。核心方案基于 NVIDIA 的 NeMo Data Designer 框架，通过两套差异化的流水线实现：针对 12 种语言，采用 Gemma-4-31B-it 模型进行全文档翻译，并引入受 MQM 启发的评分机制，对翻译质量低于 75 分的输出进行自动修复；针对其余 10 种语言，则结合 Indic Translate 模型与窗口化处理技术以确保长文档的翻译质量。所有合成数据均保留了原始文档的溯源信息，并支持通过开源的生成配方进行复现与定制。实验表明，将该合成数据与自然语言文本混合进行持续预训练，显著提升了模型在知识、推理、数学及代码任务上的表现。

**「启示」** 通过开源合成数据生成流水线与评估配方，研究者能够以透明、可审计的方式解决低资源语言的数据瓶颈。这一实践证明，高质量的自动化翻译与基于反馈的修复机制是构建大规模、多语言预训练语料库的关键路径。

**标签**: `#synthetic-data`, `#multilingual-llm`, `#data-engineering`, `#indic-languages`, `#model-pretraining`

---