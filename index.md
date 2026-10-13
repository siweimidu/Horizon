---
layout: default
title: AI 日报 · 使用指南
---

<div id="lang-zh" class="lang-section" markdown="1">

# 📡 每天 5 分钟，看完 AI 圈今天发生了什么

这里是 **Horizon AI 日报** —— 一个全自动的 AI 信息雷达。
每天早上 **07:00（北京时间）**，它会替你读完 25+ 个信息源的上百条更新，
用 AI 打分筛出真正值得看的十几条，写成中英双语日报。

**全部自动运行，不需要服务器**（跑在 GitHub Actions 上）。

---

## 🚀 快速开始

| 我想… | 点这里 |
|---|---|
| 📖 看最新一期 | 页面底部「每日速递」第一条 |
| 📥 用 RSS 订阅 | [中文订阅源]({{ '/feed-zh.xml' | relative_url }}) · [英文订阅源]({{ '/feed-en.xml' | relative_url }}) · [全部]({{ '/feed.xml' | relative_url }}) |
| 🗂 翻历史归档 | 页面底部的日期列表（保留最近 20 期） |
| ⭐ 关注更新 | [GitHub 仓库](https://github.com/siweimidu/Horizon) |

---

## 📰 信息源（25+）

| 类别 | 具体来源 |
|---|---|
| **中文媒体** | 机器之心、新智元、量子位、AI 前线、AI 日报(juya)、AIHOT |
| **厂商官方** | OpenAI、Google DeepMind、Anthropic、Mistral、Cohere、Ai2 |
| **技术博客** | Hugging Face Blog、BAIR(伯克利)、MIT News AI |
| **论文速递** | Hugging Face Daily Papers、PaperWeekly |
| **行业摘要** | TLDR AI、The Rundown AI |
| **科技媒体** | The Verge AI |
| **社区热榜** | Hacker News、Reddit（r/MachineLearning · r/LocalLLaMA · r/artificial）、Telegram 频道 |
| **新闻搜索** | Google News（AI / LLM / 大模型关键词） |

> 想加源？改仓库里的 `data/config.json` 的 `sources.rss` 数组即可，格式照抄现有条目。

---

## 📖 日报怎么读（新手必看）

每一期日报由三部分组成，看懂这几个标记就能快速扫读：

### 1️⃣ 顶部目录 —— 先看这个

开头是一份**带评分的清单**，按重要程度排序。评分是 AI 打的 0–10 分：

| 分数 | 含义 | 颜色 |
|---|---|---|
| **9.0+** | 行业大事，必看 | 🔴 玫红 |
| **7.0–8.9** | 值得关注 | 🟠 橙色 |
| **5.0–6.9** | 一般资讯 | 🟡 金色 |
| **< 5.0** | 边缘内容 | ⚪ 灰色 |

想省时间：**只点开 8 分以上的**即可。

### 2️⃣ 正文条目 —— 每条包含这些块

```
### [标题](原文链接) ⭐️ 9.0/10      ← 点标题跳原文
（一段摘要：发生了什么）

rss · Ai2 News · 10月31日            ← 来源 · 站点 · 时间
「背景信息」...                        ← AI 补的上下文：这事的前因
「影响」...                            ← 这意味着什么
「社区讨论」...                        ← Hacker News / Reddit 的高赞观点
▸ 参考链接（可展开）                   ← 原始出处与延伸阅读
标签: #AI #LLM                       ← 主题标签
```

**推荐读法**：先读摘要 → 感兴趣再看「背景」和「影响」→ 想看八卦就展开「社区讨论」。

### 3️⃣ 底部 —— 无

日报到条目结束就完了，没有广告和推荐位。

### 🔧 页面小功能

- 右上角 **EN / 中文** 按钮：切换语言（会记住你的选择）
- 文章页点 EN/中文，会跳到同一期的另一语言版本
- 正文里的 `▸ 参考链接` 是折叠块，点一下展开
- 自动适配深色模式

---

## ⚙️ 工作原理

```
每天 07:00（北京时间）
      ↓
抓取 25+ 信息源（约 150 条）
      ↓
跨源去重 → AI 逐条打分（0-10）
      ↓
按分数筛选 + 分类配额平衡（中文源/大厂/博客/论文/社区 各有上限）
      ↓
对入选内容补充背景、影响、社区讨论
      ↓
生成中英双语 → 发布到本站 + 推送邮件/Telegram
```

- **去重逻辑**：同一事件被多家报道时只保留一条
- **分类配额**：防止某个热门话题刷屏，每个类别有独立上限
- **完全自动化**：GitHub Actions 定时触发，无需人工干预

---

## ❓ 常见问题

**Q：某天没更新？**
A：偶尔会。常见原因是 AI 接口当日额度用尽（免费档有限制）或源站故障。次日会自动恢复。

**Q：评分是怎么算的？**
A：AI 按 Profile（订阅画像）的评分标准逐条打分，标准包括：时效性、影响力、信息密度、是否首发等。详见 [评分系统](scoring)。

**Q：为什么有的条目没有「背景信息」？**
A：只有高分条目会触发补充分析（省额度）。分数低的一般只给摘要。

**Q：可以只要中文/只要英文吗？**
A：可以，分别订阅 [中文 RSS]({{ '/feed-zh.xml' | relative_url }}) 或 [英文 RSS]({{ '/feed-en.xml' | relative_url }})。

**Q：我也想搭一个？**
A：本项目 fork 自开源项目 [Thysrael/Horizon](https://github.com/Thysrael/Horizon)，克隆 → 配 key → 启用 GitHub Actions 即可，文档见 [配置指南](configuration)。

---

## 📚 延伸文档

- [配置指南](configuration) — AI 提供商、信息源、过滤规则、邮件/Webhook/微信推送
- [信息源采集器](scrapers) — 各类源是怎么抓的
- [评分系统](scoring) — 0-10 分的评分机制
- [Profile 指南](profiles) — 自定义「什么内容值得留、写成什么样」

</div>

<div id="lang-en" class="lang-section hidden" markdown="1">

# 📡 Your 5-minute daily AI briefing

**Horizon AI Daily** is a fully automated news radar.
Every morning at **07:00 (UTC+8)**, it reads 100+ updates from 25+ sources,
scores them with AI, and publishes a bilingual digest of the ones that matter.

**No server required** — it runs entirely on GitHub Actions.

---

## 🚀 Quick start

| I want to… | Go to |
|---|---|
| 📖 Read the latest issue | first entry in *Daily Digest* below |
| 📥 Subscribe via RSS | [Chinese]({{ '/feed-zh.xml' | relative_url }}) · [English]({{ '/feed-en.xml' | relative_url }}) · [All]({{ '/feed.xml' | relative_url }}) |
| 🗂 Browse the archive | date list at the bottom (last 20 issues) |
| ⭐ Follow the project | [GitHub repo](https://github.com/siweimidu/Horizon) |

---

## 📰 Sources (25+)

| Category | Sources |
|---|---|
| **Chinese media** | 机器之心, 新智元, 量子位, AI前线, AI日报, AIHOT |
| **Vendor blogs** | OpenAI, Google DeepMind, Anthropic, Mistral, Cohere, Ai2 |
| **Tech blogs** | Hugging Face Blog, BAIR (Berkeley), MIT News AI |
| **Papers** | Hugging Face Daily Papers, PaperWeekly |
| **Newsletters** | TLDR AI, The Rundown AI |
| **Tech press** | The Verge AI |
| **Communities** | Hacker News, Reddit (r/MachineLearning, r/LocalLLaMA, r/artificial), Telegram |
| **News search** | Google News (AI / LLM keywords) |

> Add your own: edit the `sources.rss` array in `data/config.json`.

---

## 📖 How to read an issue

### 1️⃣ Top index — start here

A **ranked list with scores** (AI-rated 0–10):

| Score | Meaning | Colour |
|---|---|---|
| **9.0+** | Major news, must read | 🔴 rose |
| **7.0–8.9** | Worth your time | 🟠 orange |
| **5.0–6.9** | Average | 🟡 gold |
| **< 5.0** | Marginal | ⚪ grey |

Short on time? **Only open the 8.0+ items.**

### 2️⃣ Each entry contains

```
### [Title](source url) ⭐️ 9.0/10      ← click to open the original
One-paragraph summary of what happened

rss · Ai2 News · Oct 31                ← source · site · time
「Background」...                       ← AI-added context
「Impact」...                           ← why it matters
「Community」...                        ← top HN / Reddit comments
▸ References (collapsible)             ← primary sources
Tags: #AI #LLM
```

**Suggested flow**: summary → background/impact if interested → expand community for hot takes.

### 🔧 Page features

- **EN / 中文** toggle in the top-right (your choice is remembered)
- On an article page the toggle jumps to the same issue in the other language
- `▸ References` blocks are collapsible
- Dark mode supported

---

## ⚙️ How it works

```
Daily 07:00 (UTC+8)
      ↓
Fetch 25+ sources (~150 items)
      ↓
Cross-source dedup → AI scores each item (0-10)
      ↓
Filter by score + per-category quotas
      ↓
Enrich selected items (background, impact, community)
      ↓
Render bilingual digest → publish here + email/Telegram
```

---

## ❓ FAQ

**Q: A day is missing?**
A: Occasionally — usually the AI free-tier quota ran out or a source was down. It recovers automatically.

**Q: How is the score computed?**
A: The AI rates each item against a profile rubric (recency, impact, information density, exclusivity). See [Scoring](scoring).

**Q: Why do some items lack a "Background" block?**
A: Only high-scoring items get enrichment (to save quota).

**Q: Can I get only one language?**
A: Yes — subscribe to [Chinese]({{ '/feed-zh.xml' | relative_url }}) or [English]({{ '/feed-en.xml' | relative_url }}) only.

**Q: Can I build my own?**
A: This site forks the open-source [Thysrael/Horizon](https://github.com/Thysrael/Horizon). Clone, add keys, enable GitHub Actions. See the [Configuration Guide](configuration).

---

## 📚 Further reading

- [Configuration Guide](configuration) — providers, sources, filtering, email/webhook/WeChat delivery
- [Scrapers](scrapers) — how each source is fetched
- [Scoring](scoring) — the 0-10 scoring mechanism
- [Profiles](profiles) — define what gets kept and how it is written

</div>

---

## 📬 每日速递 / Daily Digest

### 中文 · <a class="rss-icon" href="{{ '/feed-zh.xml' | relative_url }}" aria-label="订阅中文"><svg viewBox="0 0 448 512" xmlns="http://www.w3.org/2000/svg"><path fill="currentColor" d="M128.081 415.959c0 35.369-28.672 64.041-64.041 64.041S0 451.328 0 415.959s28.672-64.041 64.041-64.041 64.04 28.673 64.04 64.041zm175.66 47.25c-8.354-154.6-132.185-278.587-286.95-286.95C7.656 175.765 0 183.105 0 192.253v48.069c0 8.415 6.49 15.472 14.887 16.018 111.832 7.284 201.473 96.702 208.772 208.772.547 8.397 7.604 14.887 16.018 14.887h48.069c9.149.001 16.489-7.655 15.995-16.79zm144.249.288C439.596 229.677 251.465 40.445 16.503 32.01 7.473 31.686 0 38.981 0 48.016v48.068c0 8.625 6.835 15.645 15.453 15.999 191.179 7.839 344.627 161.316 352.465 352.465.353 8.618 7.373 15.453 15.999 15.453h48.068c9.034-.001 16.329-7.474 16.005-16.504z"/></svg></a>

<ul>
  {% assign zh_posts = site.posts | where: "lang", "zh" %}
  {% for post in zh_posts limit:20 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.date | date: "%Y-%m-%d" }}</a>
    </li>
  {% else %}
    <li><em>暂无内容 / No posts yet</em></li>
  {% endfor %}
</ul>

### English · <a class="rss-icon" href="{{ '/feed-en.xml' | relative_url }}" aria-label="Subscribe English"><svg viewBox="0 0 448 512" xmlns="http://www.w3.org/2000/svg"><path fill="currentColor" d="M128.081 415.959c0 35.369-28.672 64.041-64.041 64.041S0 451.328 0 415.959s28.672-64.041 64.041-64.041 64.04 28.673 64.04 64.041zm175.66 47.25c-8.354-154.6-132.185-278.587-286.95-286.95C7.656 175.765 0 183.105 0 192.253v48.069c0 8.415 6.49 15.472 14.887 16.018 111.832 7.284 201.473 96.702 208.772 208.772.547 8.397 7.604 14.887 16.018 14.887h48.069c9.149.001 16.489-7.655 15.995-16.79zm144.249.288C439.596 229.677 251.465 40.445 16.503 32.01 7.473 31.686 0 38.981 0 48.016v48.068c0 8.625 6.835 15.645 15.453 15.999 191.179 7.839 344.627 161.316 352.465 352.465.353 8.618 7.373 15.453 15.999 15.453h48.068c9.034-.001 16.329-7.474 16.005-16.504z"/></svg></a>

<ul>
  {% assign en_posts = site.posts | where: "lang", "en" %}
  {% for post in en_posts limit:20 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.date | date: "%Y-%m-%d" }}</a>
    </li>
  {% else %}
    <li><em>No posts yet</em></li>
  {% endfor %}
</ul>
