# Day 10 — 早期品牌搜索反馈和持续分发

日期: 2026-06-21

阶段: 第 2 周 — 分发和日常运营

状态: 进行中

## 目标

利用 Google 里已经出现的第一批品牌搜索反馈，调整接下来的分发动作。

昨天的工作已经开始在外部出现信号：

- SandBase docs 页面已经在 Google 结果中出现。
- Peerlist 出现了 `Posts by SandBase AI` 结果，并且摘要里出现了我们的定位：

```text
SandBase AI. Agent infrastructure for developers building production AI agents.
```

这是外部 profile 策略开始生效的早期信号。

## 计划工作

- 保存 Google 结果截图，作为早期证据。
- 记录 Peerlist 被 Google 抓取 / 展示的信号。
- 观察错误第三方实体结果，并通过更强的正确实体信号压过去。
- 继续围绕 agent infrastructure 做轻量社媒互动。
- 继续推进一个高质量目录 / profile。
- 继续跟进技术 SEO 修复：blog sitemap、未来日期文章、品牌实体一致性。

## 使用工具

| 工具 | 作用 |
|------|------|
| Codex | 记录证据、梳理策略、准备当天计划 |
| Google Search | 观察品牌搜索结果 |
| Peerlist | 外部 profile 和可被索引的社交页面 |
| GitHub / Website / Blog | 正确实体信号和技术信任资产 |

## 执行记录

- Google 搜索截图显示 SandBase 相关结果开始出现：
  - SandBase Docs 结果：`JavaScript / TypeScript SDK | SandBase Docs`
  - Peerlist 结果：`Posts by SandBase AI`
  - Peerlist 摘要：`SandBase AI. Agent infrastructure for developers building production AI agents. 2 followers.`
- 这说明 Day 9 的 Peerlist profile 不只是目录动作，它已经成为可被 Google 抓取的品牌相关公开页面。
- 截图里同时出现了一个错误 / 无关的 Tracxn 结果，把另一个 "SandBase" 实体描述成 deadpooled company。
- 决策：不因为错误结果焦虑，而是用更多正确实体信号逐步压过去：
  - 官网页面
  - Docs
  - Blog articles
  - GitHub organization
  - LinkedIn company page
  - Peerlist profile
  - DevHunt / Uneed / Product Hunt profile
  - Agent Ecosystem
  - Hackathon Support
- 用户反馈 P0 SEO 问题已修复：blog sitemap、未来日期文章、品牌实体一致性。
- 已在线上验证 P0 SEO 修复：
  - `sitemap-blog.xml` 现在包含 85 个 URL，包括英文和中文的具体文章 URL。
  - 之前未来日期的 `n8n vs Dify` 文章现在显示为 `June 20, 2026`。
  - blog 列表没有发现 2026 年 6 月 21 日之后的未来日期。
  - 首页 title 已改为 `SandBase - Agent Infrastructure for Production AI Agents`。
  - 首页 description 已聚焦 production agents、sandboxed runtime、tool access、model routing、cloud sandboxes 和 unified APIs。
  - Organization JSON-LD 已使用正确实体链接：X、GitHub `sandbaseai`、LinkedIn 公司页、Peerlist、Discord。
  - `sitemap-pages.xml` 已包含 Agent Ecosystem 和各个项目详情页。
  - `Hackathon Support` 暂时还没有出现在生产环境 pages sitemap 里，等对应分支部署后需要再次检查。
- Google Search Console sitemap 跟进：
  - 已存在的不带 www sitemap index `https://sandbase.ai/sitemap-index.xml` 仍然有效，状态为 `成功`，上次读取时间是 2026 年 6 月 20 日，发现 954 个页面。
  - 2026 年 6 月 21 日提交 canonical www 版本 `https://www.sandbase.ai/sitemap-index.xml`。
  - GSC 弹窗确认已成功提交，但列表中新 www 记录初始状态显示 `无法抓取` / 未知，发现页面数为 0。
  - 决策：暂时保留两个 sitemap 记录，把 www 记录视为刚提交后的待处理状态，明天复查后再决定是否需要进一步处理。
- 目录 / 外部 profile 跟进：
  - 再次检查 DevHunt。提交入口存在，地址是 `https://devhunt.org/login`，支持 GitHub 和 Google 登录。
  - 用户完成了 DevHunt 的 Google 登录。
  - DevHunt 自动生成了带个人信息的 profile 字段，所以把可见 profile 字段改成 SandBase 公司口径：
    - full name: `SandBase AI`
    - username: `sandbaseai`
    - social URL: `https://www.linkedin.com/company/sandbaseai/`
    - bio: `SandBase AI builds agent infrastructure for developers building production AI agents: sandboxed runtime, safe tool access, model routing, APIs, and distributed compute.`
  - 打开 DevHunt 新工具表单，并准备了 SandBase 产品字段：
    - tool name: `SandBase`
    - slogan: `Agent infrastructure for production AI agents`
    - website: `https://www.sandbase.ai`
    - GitHub: `https://github.com/sandbaseai`
    - description: `SandBase is agent infrastructure for developers building production AI agents. It provides the runtime layer for agent apps: sandboxed execution, safe tool access, model routing, APIs, and distributed compute for agent workloads.`
  - 检查 DevHunt launch week 选项，当前可选 launch week 均显示 `$49`，超过当前 30 美金预算。
  - 决策：今天不 schedule / submit DevHunt。保留已准备好的文案，除非后续发现免费选项或预算规则变化，否则先不做付费 launch。
  - 打开 Uneed，作为今天继续推进的目录目标。
  - 在 Uneed waiting-line editor 创建 SandBase 产品草稿。
  - Uneed 先从官网自动生成草稿，再手动把文案调整回 SandBase 的核心定位。
  - 当前 Uneed 草稿：
    - name: `SandBase`
    - slug: `sandbase`
    - URL: `https://www.sandbase.ai`
    - category: `Development`
    - pricing: `Freemium`
    - tags: `API & Data`, `AI`, `Development`
    - tagline: `Agent infrastructure for developers building production AI agents.`
  - 产品草稿已保存成功，Uneed 页面提示 `Product updated`。
  - 已检查 preview mode。预览页正确展示 SandBase logo、tagline、category、pricing、tags，以及带 Uneed referral 参数的官网链接。
  - 没有使用付费的 `Submit to 100+ directories`。
  - 暂时没有安排 launch 日期。
- LinkedIn 公司页分发跟进：
  - 围绕 Uneed 发布准备和 SandBase 的 production-agent 定位，准备了一条公司页动态。
  - 使用本地图片生成流程 `scripts/generate-images-sandbase.py` 生成配图。
  - 生成图片：`assets/generated-images/linkedin-uneed-agent-infra.png`。
  - 用户手动把图片插入 LinkedIn 公司页动态。
  - 发布前把文案收短，让它更像产品更新，而不是运营流水账：
    - 开头问题：`What breaks first when AI agents move from demo to production?`
    - 产品背景：`We are preparing SandBase for a small launch on Uneed.`
    - 定位：面向 production AI agents 的 agent infrastructure。
    - 能力点：sandboxed runtime、safe tool access、model routing、distributed compute。
  - 该动态已经出现在 LinkedIn 公司页 published 列表里。
- LinkedIn 运营账号隐私加固：
  - 运营账号用于后台管理，但公开活动应该代表公司，而不是私人个体。
  - 发布后复查并收紧了必要的隐私设置。
  - 原则：公司渠道可以公开；运营账号细节保持私密、低可见、不做个人背书。

## 创建或更新的链接

- 证据截图：[Google brand result with Peerlist](../../assets/google-brand-result-peerlist-2026-06-21.png)
- LinkedIn 配图：[linkedin-uneed-agent-infra.png](../../assets/generated-images/linkedin-uneed-agent-infra.png)
- Peerlist profile/posts surface: https://peerlist.io/sandbase
- Uneed 草稿 slug 已准备：`sandbase`

## 问题 / 阻塞

- 错误的 Tracxn 实体结果可能还会存在一段时间，直到 Google 对新的 SandBase.ai 实体有更强信心。
- 明天需要在 Google Search Console 里复查新提交的 `https://www.sandbase.ai/sitemap-index.xml`。
- `Hackathon Support` 部署后需要再次检查，确认它出现在 `sitemap-pages.xml` 中。
- 需要继续做正确的第三方 profile 信号，不能只依赖官网内容。
- 需要决定 Uneed 是现在 schedule launch，还是等 launch assets 更完整后再发布。
- 后续需要判断 DevHunt 的 $49 launch 是否值得做；按当前 30 美金预算规则，暂时不做。

## 经验

早期品牌搜索结果不只是排名问题，本质是实体识别问题。

今天最重要的信号是：

```text
Google 正在开始把 SandBase AI 和 "agent infrastructure for developers building production AI agents" 联系起来。
```

下一步要做的是让这个关联更强、更干净。

不要追求每个目录都提交。要做少量高信任页面，并且反复表达同一个定位。

## 下一步

今天：

- 明天复查 Google Search Console 里新提交的 www sitemap index。
- 在 X / Peerlist 做 2-3 次围绕 production agents 的轻互动。
- 决定 Uneed 是马上排期，还是等 launch assets 准备好后再排期。
- 准备一条围绕 Agent Ecosystem 或 Hackathon Support 的产品视角内容。
