# Content Standard

This repository is not a checklist dump.

Each daily log should read like an operating journal: enough context for a reader to understand the business situation, the decision, the tools, the execution, and the lesson.

The reader should be able to picture the day: what the founder was trying to do, how Codex helped, where the browser was used, which decisions were made, which actions required human confirmation, and what changed publicly by the end of the session.

## Daily Log Structure

Each day should include:

1. Context
   - What stage the project was in
   - What was already true before the day started
   - What constraint or uncertainty mattered

2. Goal
   - One clear goal for the day
   - Why that goal mattered in the 30-day arc

3. Tools Used
   - Tool name
   - What it was used for
   - Whether it was manual, automated, or assisted
   - Any safety/privacy notes

4. How Codex Helped
   - What was delegated to Codex
   - What Codex inspected or drafted
   - What required user confirmation
   - What Codex refused to shortcut
   - What the human still had to decide

5. What We Did
   - Specific actions
   - Links created or updated
   - Files changed or assets produced

6. Decisions
   - What we chose to do
   - What we chose not to do
   - Why

7. Output
   - Public links
   - Internal artifacts
   - Drafts
   - Screenshots if appropriate

8. What We Learned
   - Things that worked
   - Things that were blocked
   - Risks discovered

9. Replicable Playbook
   - Concrete steps another founder could follow
   - What to prepare first
   - What to avoid

10. Next Actions
   - The handoff to the next day

## Tone

Use plain operator language.

Good:

- "We did not launch Product Hunt today because the gallery and launch-day reply plan were not ready."
- "We created a GitHub resource repo because developer-trust backlinks are more durable than directory submissions."
- "Codex drafted the LinkedIn company description, but the founder confirmed before public save."
- "The browser flow exposed a privacy concern: a personal LinkedIn account should not be publicly tied to the company."

Bad:

- "Submitted to 10 directories."
- "SEO improved."
- "Built brand awareness."
- "Used AI to do marketing."
- "Set up social media."

## Tool Labels

Use these labels consistently:

- `Manual`: done by a human in browser or product UI
- `Codex-assisted`: drafted, edited, audited, or operated with Codex
- `Browser-assisted`: performed through a browser with confirmation before external side effects
- `Kimi-assisted`: research or strategy generated from Kimi workspace materials
- `GitHub`: repository, commit, issue, or public code asset
- `Search Console`: indexing and crawlability checks
- `LinkedIn`: company page or social proof
- `X`: build note or technical interaction
- `Discord`: community discussion or support entry point

## Privacy Rules

Do not publish:

- Personal emails
- Login flows
- Private account identity details
- API keys, tokens, billing data
- Internal screenshots that expose user/account data
- Private Discord or LinkedIn messages

It is okay to publish:

- Public links
- Public company pages
- Public GitHub repos
- Tool categories
- Process descriptions
- Lessons learned
