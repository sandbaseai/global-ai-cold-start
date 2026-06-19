# Day 8 — Building the First Trust Layer: LinkedIn, GitHub, and a Real Backlink Asset

Date: 2026-06-19

Stage: Week 2 — Trust and external presence

Status: Completed

## Context

By this point, SandBase already had the basic website foundation in place:

- Homepage
- Docs
- Blog
- Sitemap
- Google Search Console
- Core SEO checks
- Early technical content plan

The next problem was not "how do we get more traffic tomorrow?"

The real problem was credibility.

If a developer, investor, potential customer, or Google crawler looked up SandBase, would it look like a real infrastructure company or just another anonymous AI tool page?

That question shaped the day.

## Goal

Create the first external trust layer for SandBase:

1. A public LinkedIn company page
2. A first official company post
3. A GitHub resource repository that creates a natural developer backlink
4. A reusable content asset for future Dev.to, Reddit, Hacker News, and LinkedIn posts

The goal was not to submit SandBase to as many directories as possible. The goal was to build assets that a technical audience would not immediately dismiss.

## Tools Used

| Tool | Role | How it was used |
|------|------|-----------------|
| Codex | Ops lead and browser co-pilot | Drafted page copy, operated browser flows, prepared repo files, kept an execution log |
| Browser | Live website/account operations | Created and edited LinkedIn company page, checked directory submission entrances |
| LinkedIn | B2B social proof | Company page, public profile, first official post |
| GitHub | Developer trust and backlink asset | Created `awesome-native-agent-platforms` under `sandbaseai` |
| Kimi workspace | Strategy material | Provided backlink plan, submission kit, PH/HN/Reddit drafts |
| Local Markdown docs | Operating memory | Stored decisions, logs, reusable copy, and publish-ready assets |

## How Codex Helped

This day was a good example of using Codex as an operating partner rather than just a code generator.

Codex helped in five ways:

1. **Strategy filter**

   The original backlink list contained many possible channels: Product Hunt, Hacker News, Reddit, SaaSHub, AlternativeTo, Dev.to, Crunchbase, RapidAPI, Postman, and more.

   Codex did not treat this as a checklist to execute blindly. It separated the channels into:

   - Safe to do now
   - Prepare but do not publish yet
   - Needs login
   - Blocked by verification
   - Too risky for day-one promotion

2. **Browser operator**

   Codex used the browser to operate LinkedIn and inspect submission pages. When a step would create a public side effect, such as publishing a LinkedIn post or adding an admin, Codex paused and asked for confirmation.

3. **Copy editor**

   Codex drafted LinkedIn copy and then adjusted the tone. The final positioning stayed clear and restrained:

   ```text
   Agent infrastructure for production AI agents
   ```

   This was better than overclaiming with "the only" or "revolutionary" language too early.

4. **Privacy guard**

   A key issue appeared during LinkedIn setup: the founder did not want a large personal LinkedIn account to be visibly associated with SandBase.

   Codex helped reason through what is public and what is only visible internally:

   - Public visitors see the company page as SandBaseAI.
   - Public posts show SandBaseAI as the author.
   - LinkedIn internally knows which admin performed the action.
   - The admin list is not visible to ordinary page visitors.

   This changed how the page was operated and prevented accidental personal-brand exposure.

5. **Asset builder**

   Codex created the first GitHub resource repo, not as a marketing dump but as a curated technical list.

   That was the most important strategic move of the day.

## What We Did

### 1. Created and completed the LinkedIn company page

Public page:

https://www.linkedin.com/company/sandbaseai/

The page was set up with:

- Logo
- Tagline
- Website
- Industry
- Company size
- Company type
- About section
- Message button
- Website CTA

The About copy focused on SandBase as an agent infrastructure platform:

```text
SandBaseAI is an agent infrastructure platform for developers building production AI agents.
```

The positioning was intentionally practical. The page did not try to sound like a consumer AI tool or a general AI directory.

### 2. Published the first official LinkedIn company post

The first post introduced the company page and the core infrastructure theme:

```text
Today we set up SandBaseAI's LinkedIn page.

We're building agent infrastructure for developers working on production AI agents: sandboxed runtime, tool access, model routing, and distributed compute for agent workloads.

The goal is simple: help agents move from demos to reliable systems that can run, use tools, and scale with clearer boundaries.

More soon.
```

Important detail:

The post was published as **SandBaseAI**, not reposted from the founder's personal profile.

This matters because early infrastructure brands should build a company identity, not accidentally route all attention through a personal account that may need privacy separation.

### 3. Tried to add the operating LinkedIn account as an admin

The target operating account was:

https://www.linkedin.com/in/denial-denial-ab0b98417/

The account followed the SandBaseAI page, and LinkedIn showed `1 follower`.

However, when searching inside the Page admin dialog, LinkedIn returned many ambiguous accounts named `denial denial`, but not the exact profile with:

```text
Engineer at SandBaseAI
```

Decision:

Do not select an ambiguous same-name account.

Reason:

Adding the wrong LinkedIn account as admin is a real permission mistake. Codex stopped instead of guessing.

Next action:

Retry after LinkedIn search indexing catches up.

### 4. Built the GitHub resource repo

Repository:

https://github.com/sandbaseai/awesome-native-agent-platforms

Commit:

```text
447b859 Initial awesome native agent platforms list
```

This repo is not product code. It is a developer resource asset.

The repo curates tools around:

- Agent infrastructure
- Agent runtimes
- Sandboxed execution
- Browser infrastructure
- Model routing
- Protocol and tool integration
- Agent frameworks

It includes SandBase, but it also includes other tools such as E2B, Browserbase, Modal, LiteLLM, OpenRouter, MCP, LangGraph, Dify, and n8n.

That distinction matters.

If the repo only talked about SandBase, it would look like an ad. By making it a useful ecosystem list, it becomes something developers may actually bookmark, reference, or contribute to.

### 5. Prepared a Dev.to article draft

Draft title:

```text
Your Agent Needs a Runtime, Not Just a Model
```

The first version from the strategy pack was too aggressive. It used strong claims and numbers that should not be published without proof.

Codex rewrote it into a calmer developer essay:

- Less hype
- Fewer hard claims
- More architecture framing
- One natural SandBase link
- Clear explanation of runtime, sandbox, browser, model routing, and tool integration

It was not published because Dev.to required login.

### 6. Checked directory and launch channels

The day included quick checks of several channels:

| Channel | Result | Decision |
|---------|--------|----------|
| SaaSHub | Cloudflare challenge | Do not bypass, retry manually later |
| AlternativeTo | Cloudflare challenge | Do not bypass, retry manually later |
| Product Hunt | Cloudflare challenge | Defer launch anyway |
| BetaList | old submit URL returned 404 | Find current submission path later |
| Dev.to | login required | Keep draft ready |
| GitHub | available | Publish repo |

## Decisions

### We did not launch Product Hunt

Product Hunt is a launch window, not a directory.

We deferred it because we did not yet have:

- Gallery images
- Demo screenshots
- Maker plan
- First comment
- Launch-day support plan
- Clear offer

Burning Product Hunt too early would trade a long-term launch moment for a weak backlink.

### We did not post on Hacker News

Hacker News is high leverage but unforgiving.

We did not have the right technical demo or founder reply plan ready yet. A Show HN post should happen when there is something substantial to inspect and discuss.

### We did not spam Reddit

Reddit should start with participation, not promotion.

The better move is to first comment in relevant threads around agent runtime, sandboxing, browser automation, MCP, and production agents.

### We did publish GitHub first

GitHub was the right move because it created a durable developer asset without needing a launch moment.

It also gave future posts something useful to reference:

```text
I put together a list of native agent infrastructure tools...
```

That is a better opener than:

```text
Please check out my startup.
```

## Output

Public outputs:

- LinkedIn company page: https://www.linkedin.com/company/sandbaseai/
- First LinkedIn company post
- GitHub resource repo: https://github.com/sandbaseai/awesome-native-agent-platforms

Internal outputs:

- Dev.to article draft
- Backlink execution tracker
- Submission notes
- GitHub repo copy
- Public build-log repo plan

## What We Learned

### 1. External trust starts before traffic

Before chasing distribution, a B2B infrastructure product needs credible public surfaces:

- Website
- Docs
- Blog
- LinkedIn
- GitHub
- Technical writing

Each one reduces doubt.

### 2. A backlink is better when it is also an asset

The GitHub repo is a backlink, but that is not its only purpose.

It is also:

- A developer resource
- A future content anchor
- A community contribution surface
- A way to frame SandBase inside a category

### 3. AI assistance needs confirmation boundaries

Codex can draft, inspect, operate, and organize. But public actions still need human confirmation:

- Publishing a LinkedIn post
- Creating a GitHub repo
- Adding admins
- Submitting forms
- Posting community content

That confirmation boundary is what makes AI-assisted ops usable without becoming reckless.

### 4. Privacy is part of operations

The LinkedIn admin question was not a small detail.

For founders with multiple accounts, personal accounts, or stealth concerns, social setup needs privacy decisions:

- What is public?
- What is internal?
- Which account should operate daily?
- Which account should stay hidden?
- What happens if a post is shared to a personal profile?

These decisions should be made before posting, not after.

## Replicable Playbook

If you are building a B2B AI infrastructure company from zero, this is the playbook from today:

1. Create a LinkedIn company page.
2. Fill it with restrained infrastructure positioning.
3. Publish one official company post.
4. Avoid reposting from personal accounts if privacy matters.
5. Create one GitHub resource asset that is useful beyond your product.
6. Link your website naturally from that asset.
7. Prepare technical article drafts before submitting directories.
8. Defer Product Hunt and HN until you have launch assets and reply bandwidth.
9. Treat Reddit as a place to participate before linking.
10. Keep an execution log of decisions, not just tasks.

## Next Actions

For the next day:

- Retry adding the operating LinkedIn account as a Page admin.
- Add description, homepage, and topics to the GitHub repo.
- Publish the Dev.to article after login.
- Manually retry SaaSHub and AlternativeTo.
- Start three lightweight interactions across X, LinkedIn, and Discord.

