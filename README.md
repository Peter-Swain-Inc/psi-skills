# PSI Skills Library

Pete Swain's canonical library of 25 operational skills for AI-powered entrepreneurship. Install these into any Hermes agent to get a fully equipped AI sidekick for traffic, leads, sales, and day-to-day operations.

All skills are industry-agnostic — built for any business owner using Hermes.

---

## How to Install

**Step 1 — Add the tap (once)**

```bash
hermes skills tap add github.com/Peter-Swain-Inc/psi-skills
```

> ⚠️ **If your agent says it can't find the skill or can't install it**, this is a known quirk with how Hermes handles tap repo names. The fix is to use the full identifier format directly:
>
> ```bash
> hermes skills install Peter-Swain-Inc/psi-skills/podcast-scout
> ```
>
> Just swap `podcast-scout` for whichever skill you want. See the full list below.
>
> Also make sure you have a `GITHUB_TOKEN` set in your `~/.hermes/.env` file — without it you'll hit GitHub's rate limit (60 requests/hour) and installs will silently fail. Get a token at [github.com/settings/tokens](https://github.com/settings/tokens) (no special scopes needed for public repos) and add:
> ```
> GITHUB_TOKEN=ghp_yourtoken
> ```

**Step 2 — Browse what's available**

```bash
hermes skills browse
```

**Step 3 — Install a skill**

```bash
# Short form (requires tap to be working correctly)
hermes skills install podcast-scout

# Full form (always works)
hermes skills install Peter-Swain-Inc/psi-skills/podcast-scout
```

**Step 4 — Load it in a session**

```
/skill podcast-scout
```

**Keep skills up to date**

```bash
hermes skills update
```

---

## Troubleshooting

**"Could not fetch skill from any source"**
Use the full identifier: `hermes skills install Peter-Swain-Inc/psi-skills/<skill-name>`

**"GitHub API rate limit exhausted"**
Add `GITHUB_TOKEN=ghp_yourtoken` to `~/.hermes/.env`. Free personal access token, no scopes needed.

**"Install cancelled" / nothing happens**
The install prompt requires a `y` confirmation. If you're running via an agent, ask it to pipe the confirmation: `echo "y" | hermes skills install Peter-Swain-Inc/psi-skills/<skill-name>`

**Skill not showing in `/skill` autocomplete after install**
Run `/reload-skills` in your Hermes session to pick up newly installed skills without restarting.

---

## The 25 Skills

### 🚦 Traffic (Skills 1–5)

| # | Skill | Install | Output |
|---|-------|---------|--------|
| 1 | **Podcast Scout** — Find 5 podcasts to pitch, draft outreach emails, ask before sending | `Peter-Swain-Inc/psi-skills/podcast-scout` | ⚡ Execute (ask first) |
| 2 | **Content Repurposer** — Spin one piece of content into 5 formats (LinkedIn, Twitter, video, email, carousel) | `Peter-Swain-Inc/psi-skills/content-repurposer` | 📄 Push → Google Doc |
| 3 | **Collab Scout** — Find 5 collaboration/guest post/PR opportunities, draft pitches, ask before sending | `Peter-Swain-Inc/psi-skills/collab-scout` | ⚡ Execute (ask first) |
| 4 | **Social Content Builder** — Build a full week of social content from one core idea | `Peter-Swain-Inc/psi-skills/social-content-builder` | 📄 Push → Google Doc |
| 5 | **Community Mapper** — Map 5 communities where your ideal customer lives, with how to show up in each | `Peter-Swain-Inc/psi-skills/community-mapper` | 💬 Chat |

### 🎯 Leads (Skills 6–10)

| # | Skill | Install | Output |
|---|-------|---------|--------|
| 6 | **Lead Magnet Stress-Test** — Brutal 5-point audit of your lead magnet with rewrite of headline and promise | `Peter-Swain-Inc/psi-skills/lead-magnet-stress-test` | 💬 Chat |
| 7 | **Nurture Sequence Writer** — Write a 5-email nurture sequence from a topic or offer | `Peter-Swain-Inc/psi-skills/nurture-sequence-writer` | 📄 Push → Google Doc |
| 8 | **Warm Prospect Surfacer** — Surface 5 warm prospects with follow-up messages, ask before sending | `Peter-Swain-Inc/psi-skills/warm-prospect-surfacer` | ⚡ Ask first |
| 9 | **Landing Page Auditor** — 7-point audit of your landing page with a prioritised 3-fix list | `Peter-Swain-Inc/psi-skills/landing-page-auditor` | 💬 Chat |
| 10 | **Cold List Re-Engager** — Write a 3-email comeback sequence to wake up a dead list | `Peter-Swain-Inc/psi-skills/cold-list-re-engager` | 📄 Push → Google Doc |

### 💰 Sales (Skills 11–15)

| # | Skill | Install | Output |
|---|-------|---------|--------|
| 11 | **Sales Call Prep** — Research prospect, generate discovery questions, surface objections to prepare for | `Peter-Swain-Inc/psi-skills/sales-call-prep` | 📄 Push → Notion / Google Doc |
| 12 | **Proposal Writer** — Turn rough call notes into a structured proposal + cover email | `Peter-Swain-Inc/psi-skills/proposal-writer` | 📄 Push → Google Doc |
| 13 | **Post-Call Debrief** — 5-minute brain dump after a call → decision, objections, next steps | `Peter-Swain-Inc/psi-skills/post-call-debrief` | 💬 Chat |
| 14 | **Objection Playbook Builder** — Build a full objection playbook with 3-part response scripts | `Peter-Swain-Inc/psi-skills/objection-playbook-builder` | 📄 Push → Google Doc |
| 15 | **Inbox Opportunity Scout** — Scan 30 days of inbox for buying signals, push shortlist to Slack | `Peter-Swain-Inc/psi-skills/inbox-opportunity-scout` | ⚡ Execute → Slack |

### ⚙️ Generic (Skills 16–20)

| # | Skill | Install | Output |
|---|-------|---------|--------|
| 16 | **Morning Briefing** — Daily briefing: weather, calendar, tasks, AI news, urgent emails | `Peter-Swain-Inc/psi-skills/morning-briefing` | 📲 Push → Telegram |
| 17 | **North Star Setter** — Weekly 5-question focus session → north star card pushed to Notion + Slack | `Peter-Swain-Inc/psi-skills/north-star-setter` | 📄 Push → Notion + Slack |
| 18 | **Weekly Review** — End-of-week wins, losses, energy, decision quality, and carries-forward | `Peter-Swain-Inc/psi-skills/weekly-review` | 💬 Chat |
| 19 | **Decision Support** — Thinking partner that surfaces assumptions, trade-offs, and gives one recommendation | `Peter-Swain-Inc/psi-skills/decision-support` | 💬 Chat |
| 20 | **Difficult Message Drafter** — Draft a hard message in 3 versions (direct / diplomatic / firm) | `Peter-Swain-Inc/psi-skills/difficult-message-drafter` | 📄 Push → email / Slack |

### 🧘 Personal (Skills 21–25)

| # | Skill | Install | Output |
|---|-------|---------|--------|
| 21 | **Email Spring Clean** — Find top 5 noise senders, archive and filter on confirmation | `Peter-Swain-Inc/psi-skills/email-spring-clean` | ⚡ Execute |
| 22 | **Daily Shutdown** — 5-minute end-of-day ritual: clear today, lock in tomorrow's #1, let go of one thing | `Peter-Swain-Inc/psi-skills/daily-shutdown` | 💬 Chat |
| 23 | **Agent Trainer** — Guided Q&A that builds a personalised agent profile, saved to memory | `Peter-Swain-Inc/psi-skills/agent-trainer` | 💬 Chat → Memory |
| 24 | **Morning Momentum** — 3 questions to prime the day and set one clear intention | `Peter-Swain-Inc/psi-skills/morning-momentum` | 💬 Chat |
| 25 | **Daily Read** — Find one worthwhile article today and push it to Slack with the insight worth stealing | `Peter-Swain-Inc/psi-skills/daily-read` | 📲 Push → Slack |

---

## Output Mode Key

| Symbol | Mode | Description |
|--------|------|-------------|
| 💬 | Chat | Stays in the conversation — no external output |
| 📄 | Push → Doc | Pushes content to Google Doc or Notion |
| 📲 | Push → Platform | Pushes to Telegram, Slack, or email |
| ⚡ | Execute | Takes direct action (confirm before irreversible steps) |
| ⚡ Ask first | Ask first | Surfaces options in chat, then asks before executing |

---

## About

Built by [Pete Swain](https://www.peterswain.com) — AI entrepreneur, founder of PSI Momentum and Abundance.

These skills are designed for founders and business owners running on Hermes. They're opinionated, action-biased, and built to push output to the right place — not just generate text in chat.
