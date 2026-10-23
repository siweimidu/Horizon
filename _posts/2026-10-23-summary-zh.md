---
layout: default
title: "Horizon Summary: 2026-10-23 (ZH)"
date: 2026-10-23
lang: zh
---

> 从 107 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Nintendo Switch 2 越狱技术分析](#item-tech-news-1) ⭐️ 9.0/10
2. [微软推出 MAI-DxO AI 诊断系统，模拟专家联合会诊](#item-tech-news-2) ⭐️ 9.0/10
3. [艾伦人工智能研究所 \(Ai2\) 的字节级语言模型 Bolmo 研究发表于《自然》](#item-tech-news-3) ⭐️ 9.0/10
4. [甲骨文发布 Java SE 高危漏洞安全警报](#item-tech-news-4) ⭐️ 9.0/10
5. [DNS 解析服务商 Quad9 因法律压力退出法国市场](#item-tech-news-5) ⭐️ 8.0/10
6. [NVIDIA 发布 OpenShell：用于自主 AI 代理的安全运行时环境](#item-tech-news-6) ⭐️ 8.0/10
7. [Microsoft 与 Hugging Face 发布 ThinkingBox-Training 框架](#item-tech-news-7) ⭐️ 8.0/10
8. [多家主流软件平台在 48 小时内集中披露高危安全漏洞](#item-tech-news-8) ⭐️ 8.0/10
9. [OpenAI 据报道正洽谈以 1.25 万亿美元估值融资至多 300 亿美元](#item-tech-news-9) ⭐️ 8.0/10
10. [Ai2 发布 Olmo-core 3：用于混合专家模型训练的开源基础设施](#item-tech-news-10) ⭐️ 8.0/10

**科技博客**
1. [利用数据库状态作为强化学习奖励提升智能体可靠性](#item-tech-blog-1) ⭐️ 9.0/10
2. [集成 IBM Granite 时间序列模型进行预测](#item-tech-blog-2) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Nintendo Switch 2 越狱技术分析](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) ⭐️ 9.0/10

研究人员通过自动化硬件接口成功实现了对 Nintendo Switch 2 的越狱，该过程利用了特定的安全漏洞获取了文件系统的读写权限。此项技术利用 JetKVM 进行视频输出与控制器输入模拟，并结合外部物理装置（如智能开关机器人）实现了对设备崩溃后的自动重启与持续测试。

hackernews · ledoge · 10月22日 08:01 · [社区讨论](https://news.ycombinator.com/item?id=50192536)

**「背景信息」** 任天堂 Switch 2 的 ns2jb 漏洞利用了早期软件环境中的安全缺陷，允许用户在受限的系统模块权限下运行任意代码。此前，任天堂 Switch 的破解通常依赖于硬件漏洞或特定的软件入口，而此次 ns2jb 标志着该系列新一代主机首次出现软件层面的越狱方案。

**「影响」** 此次越狱可能导致 Switch 2 游戏镜像被快速提取并泄露，进而推动游戏在非官方硬件上的模拟或重编译运行，这对任天堂的独占策略构成了潜在的商业威胁。

**「社区讨论」** 社区成员对利用 AI 辅助自动化硬件测试的流程表示赞赏，并指出这种结合 KVM 和物理自动化工具的方法显著提升了逆向工程的效率。同时，部分用户讨论了该技术对游戏版权保护的负面影响，以及 AI 工具在安全研究中存在的访问限制问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/">pepsipu . com / blog / 2026 - 10 - switch 2 - jailbreak - ns 2 jb</a></li>
<li><a href="https://gbatemp.net/threads/switch-2-jailbreak.685692/">https:// pepsipu . com / blog / 2026 - 10 - switch 2 - jailbreak - ns 2 jb / Good...</a></li>
<li><a href="https://www.androidauthority.com/nintendo-switch-2-software-jailbreak-3727013/">Nintendo Switch 2 jailbreak could open the door to a world of mods</a></li>

</ul>
</details>

**标签**: `#security`, `#hardware`, `#reverse-engineering`, `#gaming`, `#embedded-systems`

---

<a id="item-tech-news-2"></a>
### [微软推出 MAI-DxO AI 诊断系统，模拟专家联合会诊](https://aihot.news/items/ucpg7qczx7pzkl3eim00w7xgg) ⭐️ 9.0/10

微软发布了名为 MAI-DxO（Microsoft AI Diagnostic Orchestrator）的 AI 诊断系统，该系统通过编排多个 AI 智能体模拟医生专家联合会诊流程。在处理复杂病例时，该系统能够协同进行问诊、开具检查并研判诊断，在《新英格兰医学杂志》（NEJM）相关测试中达到了 83% 的准确率。

rss · AIHOT 全站 · 10月22日 23:23

**「背景」** 此前，AI 在医疗领域的应用多依赖于单一模型进行诊断，但面对复杂病例时往往难以达到临床诊断的准确度。MAI-DxO 通过引入多智能体编排技术，模拟专家联合会诊流程，旨在解决单一模型在处理复杂医学逻辑时的局限性。

**「影响」** 该系统的多智能体编排架构为医疗诊断提供了一种新的自动化辅助路径，有望通过模拟多学科会诊模式提升复杂疾病的诊断效率与准确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/the-path-to-medical-superintelligence/">The Path to Medical Superintelligence | Microsoft AI</a></li>
<li><a href="https://www.geekwire.com/2025/ai-vs-mds-microsoft-ai-tool-outperforms-doctors-in-diagnosing-complex-medical-cases/">AI vs. MDs: Microsoft tool hits 85.5% accuracy in tough diagnoses</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Healthcare AI`, `#Multi-Agent Systems`, `#Medical Diagnostics`, `#Microsoft`

---

<a id="item-tech-news-3"></a>
### [艾伦人工智能研究所 \(Ai2\) 的字节级语言模型 Bolmo 研究发表于《自然》](https://allenai.org/blog/bolmo-nature) ⭐️ 9.0/10

艾伦人工智能研究所 \(Ai2\) 开发的字节级语言模型 Bolmo 的相关研究已正式发表于《自然》期刊。该模型架构摒弃了传统的词元化 \(tokenization\) 处理方式，直接在字节层面进行操作，旨在解决现有大语言模型在多语言处理和跨领域任务中的局限性。

rss · Ai2 News · 10月31日 00:00

**「背景信息」** 传统大语言模型通常依赖分词器（Tokenization）将文本转换为子词单元，这在处理多语言或跨领域任务时常受限于词表覆盖范围。Bolmo 是一种通过两阶段转换流程，将现有的子词模型适配为字节级（Byte-level）架构的开源模型系列，旨在绕过分词限制并提升模型性能。

**「影响」** 通过直接处理字节，Bolmo 架构有望提升模型在处理非标准文本、罕见语言及复杂编码任务时的性能，为开发者提供了一种摆脱词表限制的开源大模型替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2512.15586">Bolmo : Byteifying the Next Generation of Language Models</a></li>
<li><a href="https://allenai.org/blog/bolmo">Introducing Bolmo : Byteifying the next generation of language models</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Language Models`, `#Machine Learning`, `#Open Source`, `#Research`

---

<a id="item-tech-news-4"></a>
### [甲骨文发布 Java SE 高危漏洞安全警报](https://www.oracle.com/security-alerts/alert-cve-2026-91403.html) ⭐️ 9.0/10

甲骨文发布了针对 Java SE 和 GraalVM 的高危安全漏洞 CVE-2026-91403，该漏洞位于 JSSE 组件中，CVSS 评分高达 9.1。攻击者无需身份验证即可通过网络远程利用此漏洞，从而威胁数据的机密性与完整性。受影响版本包括 Java SE 8u511、11.0.33、17.0.21、21.0.13、25.0.5、27.0.1 及多个 GraalVM 版本，官方已发布补丁并敦促用户立即升级。

telegram · zaihuapd · 10月22日 12:30

**「背景信息」** JSSE（Java Secure Socket Extension）是 Java 平台中用于实现安全网络通信的核心组件，负责处理 SSL 和 TLS 协议。由于其在企业级应用中广泛用于加密传输，该组件的漏洞通常具有较高的攻击价值。

**「影响与建议」** 由于该漏洞允许未经身份验证的远程攻击，系统管理员和开发人员应立即评估受影响的生产环境，并尽快部署甲骨文提供的最新安全补丁，以防止潜在的远程代码执行或数据泄露风险。

**标签**: `#Java`, `#Cybersecurity`, `#Vulnerability`, `#Oracle`, `#Software Engineering`

---

<a id="item-tech-news-5"></a>
### [DNS 解析服务商 Quad9 因法律压力退出法国市场](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 8.0/10

公共 DNS 解析服务商 Quad9 宣布将于 2026 年 11 月 24 日起停止在法国提供服务。此举是由于法国法院强制要求其执行网站屏蔽令，Quad9 因无法完全满足此类法律要求及随之而来的罚款压力，决定撤出该市场。

hackernews · farrokhi · 10月22日 14:32 · [社区讨论](https://news.ycombinator.com/item?id=50195959)

**「背景信息」** 此前，法国媒体公司（如 Canal+ 和 beIN Sports）针对 Quad9 发起多项法律诉讼，要求其作为 DNS 解析器对特定侵权网站实施域名封锁。Quad9 此前已在德国面临类似的法律挑战，并曾因未能执行封锁令而遭到罚款，此次退出法国市场是其在面对司法强制封锁要求与维护中立性原则冲突时的最新应对措施。

**「对法国用户的实际影响」** 由于法国法院强制要求 DNS 解析器执行针对特定网站的屏蔽令，Quad9 计划于 2026 年 11 月 24 日起通过地理位置过滤（GeoIP）阻止法国境内用户访问其服务。此前，包括 Cisco Umbrella 在内的其他 DNS 提供商也曾因类似的版权诉讼和强制屏蔽要求而选择退出特定市场，这表明法国境内的用户将面临更少的公共 DNS 选择，且必须依赖于愿意遵守此类司法屏蔽令的解析器。

**「社区讨论」** 社区成员对将 DNS 解析商视为法律责任主体表示质疑，认为这类似于惩罚电话簿公司。部分用户指出，Quad9 的退出与此前思科等公司因应对体育版权方的屏蔽令而采取的类似策略一致，并讨论了地理位置过滤在规避法律风险时的局限性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quad9.net/news/press/quad9-faces-new-dns-censorship-legal-challenge-in-france-from-canal/">Quad9 Faces New DNS Censorship Legal Challenge in France from ...</a></li>
<li><a href="https://reclaimthenet.org/quad9-considers-leaving-france-over-website-blocking-order">Quad9 Considers Leaving France Over Website Blocking Order</a></li>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-will-leave-france-after-court-orders-piracy-blocking-penalty/">DNS Resolver Quad9 Will Leave France After Court Orders ...</a></li>
<li><a href="https://torrentfreak.com/dns-block-canal-sues-cloudflare-google-cisco-to-fight-piracy-231230/">DNS Block : Canal+ Sues Cloudflare, Google &amp; Cisco ... * TorrentFreak</a></li>
<li><a href="https://www.torlock.com/news/11381/court-upholds-belgian-pirate-dns-blocking-order-opendns-exit-looms.html">Court Upholds Belgian Pirate DNS Blocking Order, OpenDNS Exit ...</a></li>

</ul>
</details>

**标签**: `#DNS`, `#Internet Censorship`, `#Privacy`, `#Legal`, `#Infrastructure`

---

<a id="item-tech-news-6"></a>
### [NVIDIA 发布 OpenShell：用于自主 AI 代理的安全运行时环境](https://github.com/NVIDIA/OpenShell) ⭐️ 8.0/10

NVIDIA 推出了 OpenShell，这是一个旨在为自主 AI 代理提供安全运行环境的开源项目。该工具通过容器化技术和策略强制执行，限制代理对文件系统、网络资源和敏感凭据的访问，从而在赋予代理必要操作权限的同时降低安全风险。

hackernews · niemandhier · 10月22日 17:44 · [社区讨论](https://news.ycombinator.com/item?id=50198675)

**「背景信息」** 随着自主 AI 代理在软件开发和系统管理中的应用日益广泛，如何平衡代理执行任务所需的系统权限与数据安全成为核心挑战。此前，开发者通常依赖基础的容器化技术来隔离代理环境，但缺乏针对代理行为的细粒度策略控制和审计机制，导致代理在访问文件、网络及凭据时存在潜在的安全风险。

**「影响」** 开发者可以利用 OpenShell 为 AI 代理构建隔离的执行沙箱，从而在允许代理执行安装软件包或调用 API 等任务时，有效防止数据泄露或未经授权的系统访问。

**「社区讨论」** 社区用户普遍认可在容器中运行代理的必要性，但部分用户指出，在赋予代理高权限与确保系统安全之间始终存在权衡，仅靠运行时限制无法完全消除数据外泄风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/ai/openshell/">NVIDIA OpenShell | Open, Secure Runtime for AI Agents</a></li>
<li><a href="https://github.com/NVIDIA/OpenShell">OpenShell – private runtime for autonomous AI agents</a></li>
<li><a href="https://developer.nvidia.com/blog/how-nvidia-openshell-reference-architecture-secures-and-governs-ai-agent-workloads-at-scale/">How NVIDIA OpenShell Reference Architecture Secures and ...</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Security`, `#Containerization`, `#NVIDIA`, `#Software Engineering`

---

<a id="item-tech-news-7"></a>
### [Microsoft 与 Hugging Face 发布 ThinkingBox-Training 框架](https://aihot.news/items/c1wb4w4ehhq5ig4m4hwv3kbbp) ⭐️ 8.0/10

Microsoft 与 Hugging Face 联合发布了 ThinkingBox-Training 框架，旨在通过强化学习（RL）训练 AI 智能体。该框架将智能体执行任务后的数据库最终状态检查结果作为奖励信号，目前相关代码已在 GitHub 开源。

rss · AIHOT 全站 · 10月22日 22:24

**「背景信息」** ThinkingBox 最初于 2026 年 10 月发布，是一个包含 507 个有状态业务工作流的基准测试框架，旨在通过验证数据库的最终状态和副作用来评估智能体的执行准确性。此前，该框架主要用于评估智能体在复杂业务场景下的可靠性，而本次发布的 ThinkingBox-Training 则进一步将其扩展为支持强化学习训练的完整工具链。

**「影响」** 开发者现在可以利用数据库执行的客观验证结果来量化智能体的表现，从而解决传统强化学习中奖励函数难以设计或不够精确的问题，提升智能体在数据处理任务中的准确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://riverfrontai.com/journal/microsoft-s-thinkingbox-grades-ai-agents-on-database-state-n-3ef2c1b9">Microsoft&#x27;s ThinkingBox Grades AI Agents on Database State ...</a></li>
<li><a href="https://huggingface.co/blog/microsoft/thinkingbox">The Agent Said It Was Done. The Database Disagreed.</a></li>

</ul>
</details>

**标签**: `#Reinforcement Learning`, `#AI Agents`, `#Microsoft`, `#Hugging Face`, `#Machine Learning`

---

<a id="item-tech-news-8"></a>
### [多家主流软件平台在 48 小时内集中披露高危安全漏洞](https://aihot.news/items/bw9sz0kx1l5ousd589zo3ficm) ⭐️ 8.0/10

在过去 48 小时内，GitLab、PHP、Node.js、Chrome、Oracle 及 Atlassian 等多个主流软件平台集中披露了大量安全漏洞。其中，GitLab 被曝出 CVSS 评分达 10.0 的远程代码执行漏洞，PHP 存在未认证远程代码执行风险，Node.js 涉及 Brotli 解码器等多个缺陷，且 Chrome、Oracle 与 Atlassian 分别发布了数百至上千项安全修复与补丁。

rss · AIHOT 全站 · 10月22日 22:21

**「背景信息」** 此次集中披露的漏洞主要涉及广泛使用的基础设施组件，其中 PHP 的 CVE-2026-109618 和 CVE-2026-109619 漏洞允许攻击者在未授权情况下执行任意代码，导致服务器面临完全被控制的风险。此外，GitLab 修复的 CVE-2026-110264 漏洞同样被评定为 CVSS 10.0 极高危等级，影响自托管版本。

**「安全影响与建议」** 由于此次漏洞涉及底层基础设施与常用开发工具，相关组织与开发者需立即评估受影响的系统版本，并优先部署厂商提供的安全补丁以防范远程代码执行攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/10/critical-gitlab-flaw-cvss-100-could.html?m=1">Critical GitLab Flaw (CVSS 10.0) Could Allow Unauthenticated RCE...</a></li>
<li><a href="https://ubuntu.com/blog/php2shell-vulnerability-fixes-available">php 2shell (CVE- 2026 -109618 and CVE- 2026 -109619) – PHP critical ...</a></li>
<li><a href="https://www.digitalocean.com/blog/critical-php-rce-vulnerabilities-patch-now">Critical PHP RCE Vulnerabilities : Patch Now (CVE- 2026 -109618...)</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#software-engineering`, `#infrastructure`, `#devops`

---

<a id="item-tech-news-9"></a>
### [OpenAI 据报道正洽谈以 1.25 万亿美元估值融资至多 300 亿美元](https://aihot.news/items/wg3g8yf3e8c11smv9q88k4poz) ⭐️ 8.0/10

OpenAI is reportedly in talks to raise up to $30 billion at a $1.25 trillion valuation, with potential strategic partnerships involving compute resources.

rss · AIHOT 全站 · 10月22日 22:08

**标签**: `#OpenAI`, `#AI Industry`, `#Venture Capital`, `#Artificial Intelligence`, `#Corporate Strategy`

---

<a id="item-tech-news-10"></a>
### [Ai2 发布 Olmo-core 3：用于混合专家模型训练的开源基础设施](https://allenai.org/blog/olmocore3) ⭐️ 8.0/10

艾伦人工智能研究所（Ai2）发布了 Olmo-core 3，这是一套专为混合专家（MoE）语言模型设计的开源训练基础设施。该系统通过重新设计的架构，旨在提升大规模模型训练过程中的效率与可扩展性，并向研究社区提供完全透明的训练堆栈。

rss · Ai2 News · 10月31日 00:00

**「背景信息」** 混合专家模型（MoE）通过仅激活模型参数的一小部分来处理每个输入，从而在保持大规模参数量的同时降低了计算成本。此前，高效训练此类模型通常依赖于高度定制的闭源分布式计算框架，这限制了研究人员对大规模模型训练过程的透明度和可复现性。

**「对开发者的影响」** 研究人员和开发者现在可以利用 Olmo-core 3 将混合专家（MoE）模型的训练规模扩展至万亿参数级别，同时通过将数据路由至驻留专家而非重复收集权重，实现了比前代架构高出 2.7 倍的吞吐量。该工具的开源特性降低了大规模模型训练的门槛，但用户需注意，部分实验性的重叠与卸载功能可能会导致训练效率下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allenai.org/blog/olmocore3">Introducing Olmo-core 3: Open, scalable training ...</a></li>
<li><a href="https://www.unite.ai/ai2-releases-olmo-core-3-open-training-stack-for-trillion-parameter-moes/">Ai2 Releases Olmo-Core 3, Open Training Stack for Trillion ...</a></li>
<li><a href="https://www.techtimes.com/articles/328470/20261002/ai2-releases-olmocore-3-open-moe-training-stack-delivers-27x-throughput-gain.htm">Ai2 Releases OlmoCore 3: Open MoE Training Stack Delivers 2 ...</a></li>

</ul>
</details>

**标签**: `#Artificial Intelligence`, `#Machine Learning`, `#Open Source`, `#Large Language Models`, `#Distributed Systems`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [利用数据库状态作为强化学习奖励提升智能体可靠性](https://huggingface.co/blog/microsoft/thinkingbox-training) ⭐️ 9.0/10

rss · Hugging Face Blog · 10月22日 22:24

**「背景」** 在处理生产级数据库任务时，智能体往往表现出“虚假完成”的问题，即模型声称任务已解决，但实际数据库状态却未达到预期。现有的评估指标通常仅关注单次成功率，忽略了任务执行的重复性与可靠性，导致模型在面对复杂业务逻辑时缺乏生产环境所需的稳定性。

**「方案」** ThinkingBox 通过将任务执行后的最终数据库状态作为可执行的奖励信号，构建了一套强化学习训练闭环。为了解决训练数据选择难题，作者引入了“离线策略相对难度”方法，通过对基础模型进行多次探测，筛选出那些模型既非完全无法解决、也非完全掌握的“中间态”任务，从而为 GRPO 算法提供有效的对比梯度。在 Qwen3.8-27B 模型上的实验表明，通过这种方式进行 50 步强化学习微调，模型在 507 个基准测试任务中的全重复成功率（Observed 20/20）从 7.5% 提升至 21.1%，显著增强了模型在生产环境中的可靠性。此外，作者强调了训练与评估解析器的一致性，并建议在训练前通过探测分布来优化任务池，以避免无效的计算开销。

**「启示」** 提升智能体生产可靠性的关键在于从关注单次成功率转向关注重复执行的稳定性，利用可执行的数据库状态作为奖励信号能有效引导模型收敛至更稳健的执行路径。对于开发者而言，通过离线策略探测筛选训练任务，是实现模型从“偶尔成功”向“持续可靠”转化的核心手段。

**标签**: `#Reinforcement Learning`, `#Agentic Workflows`, `#Model Evaluation`, `#Database Reliability`, `#GRPO`

---

<a id="item-tech-blog-2"></a>
### [集成 IBM Granite 时间序列模型进行预测](https://huggingface.co/blog/ibm-research/granite-timeseries-ensemble-r1) ⭐️ 8.0/10

rss · Hugging Face Blog · 10月22日 07:51

**「背景」** 在时间序列预测中，预训练模型无需针对特定数据集进行微调即可直接使用，但选择最合适的模型架构往往充满挑战。不同的架构（如 PatchTST 或状态空间模型）在处理工业信号、零售需求或季节性数据时表现各异，单一模型难以在所有场景下保持稳健。

**「方案」** IBM Granite 时间序列集成（Granite Timeseries Ensemble）通过组合四种互补的 Granite 架构（PatchTST-FM-r1/r2、FlowState 和 TTM），提供了一种无需重新训练或优化权重的预测方案。该方案通过统一的接口，利用“概率集成”（Probabilistic Ensemble）或“四分位距集成”（IQR Ensemble）两种策略，将多个模型的预测结果合并为中位数和分位数输出。概率集成通过对各成员进行等权重概率池化，提供了一种简单且稳健的默认选择；而 IQR 集成则根据各成员预测区间的宽度动态调整权重。在 GIFT-Eval 基准测试中，该集成方法在 MASE 指标上优于单一模型，有效降低了因选错模型而带来的风险。尽管该方法通过并行加载多个模型增加了推理延迟和内存开销，但其模块化设计允许开发者根据需求灵活替换成员或调整聚合逻辑，从而在不同应用场景中实现性能与稳健性的平衡。

**「启示」** 通过集成多种互补的预训练架构，开发者无需预先确定最佳模型即可获得稳健的预测结果。这种方法将预测重心从“挑选单一最优模型”转向“利用模型多样性”，为处理复杂多变的时间序列数据提供了一个高效的通用起点。

**标签**: `#time-series-forecasting`, `#ensemble-learning`, `#machine-learning-engineering`, `#probabilistic-forecasting`

---