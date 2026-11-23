---
title: "Claude Code: Build Your First AI Agent in 20 Minutes (100% No Coding)"
channel: Grace Leung
url: https://www.youtube.com/watch?v=F8jidmEkIeM
date_watched: 2026-11-22
duration: 20:01
source: captions
tags: [ai, claude-code, agents, skills, memory, automation]
---

# Claude Code: Build Your First AI Agent in 20 Minutes

> **TL;DR:** A 5-level recipe for building a no-code AI agent in the Claude desktop app's Code tab: workspace → agent → skills → memory → cloud + schedule. The demo is a content-creator agent that turns videos/newsletters into on-brand animated Instagram carousels, but the method applies to any agent. Sponsored by Anthropic (Max plan).
> Follow-up to [[Grace Leung - How I'd Use Claude If I Started Today]] (its "Day 7: Custom").

## Key takeaways
- **Chatbot answers questions; an agent takes the job off your plate.** What makes it an agent is *judgment*: given a goal, it decides what to do first, which tools to use, and whether the result is good enough.
- **Five parts of every agent:** brain (model), context (what it knows), job (goal), rules (how to work / never do), tools (what it may use).
- **Workspace first (Level 0).** Same request in a prepared folder vs an empty folder gives a very different, on-brand result.
- **Skills = training manual; memory = notebook; CLAUDE.md = onboarding guide.** Agent reads all three each run.
- **Let Claude interview you** (with "think hard") to build skills and plans rather than writing them yourself.
- **Self-improvement = a memory file** that stores only *reusable* feedback, not one-off edits.
- **First versions are never final**; expect iteration, and feed corrections back into memory.
- Cloud = GitHub repo + connectors (Notion) + scheduled task, so it works with your laptop closed.

## Notes

### The 5 parts of every agent `[00:41]`
- Brain: the model doing the thinking.
- Context: brand, audience, voice, visual style.
- Job/goal: what it's working toward.
- Rules: how it should work, what it must never do.
- Tools: what it's allowed to use.
- Her example: content creator agent to turn long-form videos + newsletters into Instagram posts.

### Level 0: Set up the agent workspace `[01:25]`
- Workspace = just a **folder** (hers: "Business OS", the central home for all agents). Like prepping a desk, files and a guide before a new teammate starts.
- Put in logo, personal photos, a few real IG posts as style references.
- Claude desktop app → **Code tab** → pick folder. Two modes: **local** (your computer) and **cloud** (covered in Level 4).
- **Permission mode:** she recommends **auto mode**: works without interrupting but blocks risky actions; switchable any time.
- **Model:** Opus 5.5, chosen for precise instruction-following and design taste.
- Each Claude Code session starts from zero, so onboard it: ask Claude to read your website + files and create
  1. a **CLAUDE.md** onboarding guide (read first every time), and
  2. a **brand context** file (business, audience, voice, visual style).
  - Claude uses tools to fetch the site and asks clarifying questions (fonts, why you like the example posts).
- Test in a **new session**: "plan next week's posts about Claude Code for Marketers" → on-brand plan with her palette. Same prompt in an empty folder is generic.

### Level 1: Build your first agent `[04:59]`
- Use an **"Agent Designer" prompt** (she provides it in the video description): paste it, describe the job, and Claude interviews you then designs the agent.
- Result: a new agent folder with a `content creator agent` file covering the five parts (can skip reading it; Claude handles it).
- Invoke with **`@`** and pick the agent; give it the input (e.g. transcript) and constraints ("carousel, max 10 slides").
- Agent reads inputs, proposes angles to choose from, builds a draft. First draft had missing images and weak font sizing → give feedback, it rebuilds.
- Takeaway: rarely is v1 final; iterate.

### Level 2: Make it reliable `[07:30]`
- Problem: each run it improvises hook/layout/design. Fix: **agent skills** = a playbook of how the job is done every time.
- Build a *content playbook* skill (incl. a **motion skill** for animation):
  1. Ask Claude to **interview you** about what to improve in the post it just made (add "think hard"; it asked about brand energy and signature emotion).
  2. It writes the skill into the project's `.claude` folder with core workflow + checklist criteria.
- Test by typing **`/`** (lists installed skills) and `@` to tag a file: "animate this carousel".
- Output: each slide exported as an individual video, ready to upload as animated posts.
- To make it automatic: **assign the skill to the agent** and update **CLAUDE.md** to say "use this agent whenever I ask for social posts or carousels". Background tasks panel shows running work.
- Test on a new newsletter: it picked up the task and used the skill. Remaining flaws: off-brand brown backgrounds, lack of variety between inner slides.

### Level 3: Make it self-improving `[12:10]`
- By default every session is "day one". Give it a **memory file** next to CLAUDE.md and tell it to read it before every job.
- **Key instruction:** only save feedback that applies to future posts, not one-off edits, to avoid cluttering memory.
- Give feedback as bullets ("no brown, vary inner backgrounds") → agent fixes the post **and** writes lessons to memory.
- Second newsletter: noticeably better, no off-brand colours. New feedback (default robot icon, remove black outline on cover face) again goes into memory.
- Mental model: **onboarding guide** (day one) + **playbook** (training manual) + **memory** (notebook of lessons).
- Levels 1-3 already give a working agent; Level 4 is optional.

### Level 4: Run it in the cloud `[14:51]`
- Local limitation: laptop closed = can't reach the agent.
- Add two tools first:
  - **Notion** connector (Customize → Connectors) so drafts go to a Notion *content inbox*, then tell the agent it may use Notion.
  - **GitHub:** ask Claude to turn the Business OS folder into a **private repo** (login required; free account is fine).
- Use from the **Claude mobile app**: Code → new session → pick the repo → "check my Notion inbox and turn pending ideas into carousels for review". Runs in background (phone can be off), reports back with Notion links, marks tasks done; feedback updates memory too.

### Scheduled task / routine `[17:52]`
- Remaining gap: you still have to ask. Create a **scheduled task** ("Daily Content Drop"): runs each evening, checks Notion inbox, builds carousels, and **proposes playbook improvements from feedback**.
- Under **advanced settings**, select the repo so it runs **in the cloud** at the scheduled time → drafts wait for review next morning.

### This week's actions `[18:52]`
1. Set up workspace. 2. Build agent (job, tools, rules). 3. Add skills. 4. Add memory. 5. Move to cloud. One level at a time; same pattern for any agent.

## Terms & concepts
| Term | Meaning |
|---|---|
| Agent | AI given a goal that decides actions, tool use, and when output is good enough |
| Workspace | A folder holding files, CLAUDE.md, brand context, agents, skills |
| CLAUDE.md | Onboarding file Claude Code reads first every session |
| Agent Designer prompt | Interview-style prompt that designs an agent for you |
| Skill | Reusable playbook (workflow + checklist) the agent follows each time |
| Memory file | Notebook of reusable lessons from feedback, read before every job |
| Permission mode (auto) | Runs without constant prompts but blocks risky actions |
| Connector | Integration (Notion, GitHub…) giving the agent tools |
| Scheduled task | Recurring run, optionally in the cloud via a repo |

## Resources mentioned
- Claude desktop app: https://claude.com/download
- Agent Designer prompt: in the video description (copy it from there; not reproduced here)
- Claude Code on Max plan (sponsor link in description)
- Next video: moving from one agent to a team of agents

## Caveats & my review
- **Sponsored by Anthropic**; examples are marketing/social content, but the pattern is general.
- "Auto mode", cloud sessions, mobile Code sessions and cloud scheduled tasks may depend on plan/version; verify in your own account. Cloud scheduling needs the repo selected, as shown.
- Missing from the video, worth adding yourself:
  - **Security:** a cloud agent with GitHub + Notion access can read private data and act on it. Grant least privilege, review before publishing, and beware of prompt injection in fetched web pages/transcripts.
  - **Memory hygiene:** periodically review the memory file; it can accumulate wrong or contradictory lessons.
  - **Cost/limits:** daily cloud runs consume plan usage.
  - **Backups/versioning:** the GitHub repo doubles as version history for skills and memory.

## Open questions / to try
- [ ] Create a workspace folder + CLAUDE.md + brand/context file for something you do repeatedly (e.g. these video notes)
- [ ] Try the Agent Designer prompt, or interview-based skill creation with "think hard"
- [ ] Add a memory file with the rule "only reusable feedback"
- [ ] Try `/` skills list and `@` file/agent referencing in the Code tab
- [ ] Push a workspace to a private GitHub repo and run one session from the mobile app
- [ ] Set up one cloud scheduled task with a run summary and a failure plan (see Day 6 in the previous note)
