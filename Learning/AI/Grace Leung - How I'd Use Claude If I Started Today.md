---
title: How I'd Use Claude If I Started Today
channel: Grace Leung
url: https://www.youtube.com/watch?v=71w6Le62wk0
date_watched: 2026-11-22
duration: 21:32
source: captions
tags: [ai, claude, workflow, productivity, marketing]
---

# How I'd Use Claude If I Started Today

> **TL;DR:** Claude feels hard because it's a box of flexible building blocks, not one product. Grace Leung's advice: stop chasing features and build a *system*, following a 7-day order: Brief → Access → Method → Studio → Taste → Routine → Custom. Examples are marketing-focused, but the progression applies to any role.

## Key takeaways
- Order matters more than speed: each day builds on the last (context → tools → process → output → style → automation → custom build).
- **Projects** are the single most valuable feature: a chat gives answers, a project runs work like a mini system.
- **Projects = what Claude needs to know; Skills = how you do the work** (an SOP for Claude).
- Turn a *proven* workflow into a skill (do it a few times, then "turn what we just did into a reusable skill"), and add a scoring rubric so it self-reviews.
- Define business terms once in the project so every dashboard calculates the same way.
- Taste is the human edge: teach Claude your design rules from references, ask for variants, and lock in a master template.
- Only schedule tasks you'll actually check; always add failure planning and run summaries.
- In Claude Code: have Claude interview you and plan first, then make it test its own work.

## Notes

### Why Claude feels hard `[00:15]`
- Speaker's context: 2+ years, 3,000+ hours, 200+ projects.
- Too flexible: projects, connectors, skills, artifacts, plugins can be combined any way, so there's no single "best way".
- Mindset shift: every new feature is just another block in the system you're already building, so less overwhelm.
- She says Claude today is a complete rebuild with simpler setup. The 7 days need not be literal; the *order* matters.

### Day 1: Brief `[01:18]`
Don't open a chat. Tell Claude who you are and how you work, in two places:
- **Settings → instructions:** tone, format, no-gos (hers: no em dashes, no long explanations).
- **Memory:** built-in; learns as you chat, or just write plain words (e.g. "marketing lead at a B2B software company, selling to small business owners, working on next product launch"). Organised into editable topics (profile, brand voice, content philosophy, tools).
- **Projects:** one per client/campaign/goal with its own files, instructions and now its own **goal**.
  - Claude acts like a project manager: breaks the goal into tasks and moves work forward.
  - Example: product launch project → parallel threads for competitor research, emails, landing page, sharing the same memory.
  - Limitation: a project mainly knows only what you upload (leads into Day 2).

### Day 2: Access `[03:34]`
- Stop copy-pasting between Claude and your tools. Use **connectors**: Customize → Connectors (Gmail, Drive, Notion, HubSpot, Slack, calendar…).
- Start with only 1–2 apps where your work lives.
- **Google Workspace** is her favourite: Claude edits Docs, Sheets and Slides directly beside the chat.
  - Brainstorm and decide in chat, then Claude builds the deck/email plan in the doc.
  - Can read and reply to **comments** in a Google Doc, revise that section and resolve the thread.
- Combining tools: after a client call, read the transcript → extract action items → create tasks with owners and due dates in your PM tool.
- Other uses: catch up on a Slack channel, prep tomorrow's meeting from calendar, schedule content ideas into Notion.

### Day 3: Method `[05:59]`
- Stop writing better prompts; make **skills**: step-by-step way you do a task, with rules and success criteria.
- How to create one:
  1. Pick a workflow you've already proven (e.g. campaign recap), iterate with Claude until you'd send it unedited.
  2. In the same chat: "Turn what we just did into a reusable skill. Make it brand agnostic so I can use it in other projects."
  3. Next time Claude uses it automatically.
- Lessons after ~a year of building skills:
  - **Fix a misbehaving skill immediately**, in the same chat while context is fresh. Skills now have **version tracking / rollback**.
  - **Add a scoring rubric**: define what "good" looks like and tell the skill to score its output, fix gaps and re-score until it passes.
    - Example rubric (AI-search blog posts): headings are real questions, answer in first two sentences, every stat has a named source, at least one first-hand insight.
- Sponsor segment (HubSpot): free *Marketer's Agent Skills Pack*, five skills (content research, copywriting, strategy, data viz, landing page audit); checks brand context first; works on Claude, ChatGPT, Gemini.

### Day 4: Studio `[09:13]`
- **Artifacts** = anything Claude makes that you put in front of someone (doc, deck, dashboard, small tool). Opens beside the chat, clickable, refinable, shareable via link.
- **Dashboards** are her most-made artifact:
  - Create it *inside the project* so Claude knows your goals and metrics.
  - Connect a data source (BigQuery, Notion, HubSpot, Sheets, or upload CSV/Excel) and ask in plain English; Claude writes the query, pulls data, builds charts (e.g. stacked bar of lead type by month). Connected data stays up to date.
  - Before building, ask: **what business decision should this help make?** (not "track everything").
  - Advantage over classic Data Studio: because it lives in the project, Claude can explain *why* revenue dipped (campaigns, emails, changes made that month).
- **Tip:** Claude writes its own query per chart, so definitions (e.g. "high priority lead", "conversion") can drift. Write definitions once in the project.
- Sharing: link access respects each viewer's own data permissions.
- New: **whiteboards** (funnel teardowns, learning-path mapping to spot gaps) and **spreadsheets**.

### Day 5: Taste `[12:57]`
- AI makes anything in seconds, so *making* isn't the skill; **knowing what's good** is. Claude has "everyone's average" taste; brand colours alone don't fix layouts/spacing.
- **Claude Design** (built into Claude under Design): feed brand guidelines, past decks, assets or your website to generate a design system.
- Two ways to teach taste:
  1. Give references you love + real (non-AI) brand assets, let Claude analyse them, turn findings into **rules** in the design system. Review and add what it missed.
  2. Always ask for **several variants**; compare side by side, pick closest, refine.
- **Master template:** before any deck, plan layouts first (big number, comparison, timeline, chart…). Hers has 24+ layouts; more options means less improvising. Save it to the design system, then hand Claude a report and get a deck that auto-picks layouts.
- Same for carousels, infographics, email design, icon libraries; Claude can also do animated carousels and simple motion graphics.

### Day 6: Routine `[15:59]`
- Claude works *without* you: **scheduled tasks** run daily/weekly in the cloud even with the laptop closed. She says this replaced most of her n8n workflows.
- Examples: Monday content-idea research added to a planner; monthly SEO refresh brief for pages losing impressions; daily ad-spend checker that flags overspend and waits for approval before changing anything.
- Set up under **Scheduled**, but works best from inside a project (knows brand, skills, connectors). Ask Claude to suggest what to automate.
- Tips:
  - Only automate things you do often **and will actually check**; more tasks = more maintenance.
  - Ask Claude to plan and review before saving.
  - **Ask "what could go wrong?"** (missing data, logged-out connector) and have it handle each case.
  - Ask for a **run summary** (email/Slack/Notion/Sheets): what it did, what needs attention, what failed, so silent failures don't linger.

### Day 7: Custom `[18:23]`
- **Claude Code**: build your own agents/systems beyond the app. No coding needed; describe in plain language.
- Start: desktop app → Code tab → pick a folder (e.g. "Coding Playground") → say what to build.
- Uses: landing pages, tools that process hundreds of local files, apps connecting to your tools.
- Suggested first build: a **command center** that shows how things are going, what's waiting on you, and launches workflows in one click; can use your design system.
- Two habits:
  1. **Interview + plan first:** "Ask me questions until you fully understand what I need, then show me the plan." Changing a plan is cheaper than rebuilding (saves tokens).
  2. **Make Claude verify its own work:** it can open the build, click around like a user, and fix bugs. Tell it what matters (numbers match real reports, every button works, edge cases).
- Closing: Claude goes from chat box to a system that works for you. Next video suggested: building your first AI agent with Claude Code (https://www.youtube.com/watch?v=F8jidmEkIeM).

## Terms & concepts
| Term | Meaning |
|---|---|
| Brief | Your role, preferences and no-gos set via instructions + memory |
| Memory | Built-in, editable knowledge Claude keeps about you and your work |
| Project | Container with files, instructions and a goal; can spawn parallel threads sharing memory |
| Connector | Sign-in integration letting Claude read/write apps like Gmail, Drive, Notion, HubSpot |
| Skill | Reusable SOP telling Claude *how* to do a task, with rules and success criteria |
| Rubric | Self-scoring checklist inside a skill; Claude iterates until it passes |
| Artifact | Shareable output (doc, deck, dashboard, tool) shown beside the chat |
| Design system | Brand rules/layouts Claude Design reuses for consistent visuals |
| Master template | Saved library of slide layouts (hers: 24+) |
| Scheduled task | Recurring cloud-run job defined once |
| Command center | Single Claude Code-built screen for status, pending items and one-click workflows |

## Resources mentioned
- Marketer's Agent Skills Pack (HubSpot, free): https://clickhubspot.com/095d06 *(sponsored)*
- Claude Cowork Marketing Setup Kit: https://www.graceleung.com/claude-cowork-marketing-setup-kit/
- Next video, first AI agent with Claude Code: https://www.youtube.com/watch?v=F8jidmEkIeM
- Her paid program: AI Growth System for Marketing

## Open questions / to try
- [ ] Fill in Settings instructions + memory (Day 1) and create one project for a real goal
- [ ] Connect one connector (Drive or Gmail) and test Google Doc comment handling
- [ ] Turn one proven workflow into a skill and add a scoring rubric
- [ ] Write project-level metric definitions before building any dashboard
- [ ] Pick one weekly scheduled task with a "what could go wrong" review and run summary
- [ ] Try the "interview me, then plan" prompt in Claude Code
- Caveat: UI names (Customize, Scheduled, Claude Design, whiteboards) are as described in the video as of Nov 2026; availability may vary by plan.
