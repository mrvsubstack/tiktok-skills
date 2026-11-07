---
name: tt-profile-optimizer
description: "Audits a TikTok profile — photo, name, username, the very short bio, link, pinned videos and the first rows of the grid — and rewrites them so a viewer who just watched one video instantly knows what they'll get by following. Includes what to do before the link field unlocks. Use this skill whenever the user says things like \"fix my TikTok bio\", \"review my TikTok profile\", \"what should I pin on TikTok\", \"people watch but don't follow\", \"how do I add a link on TikTok\", or \"TikTok profile audit\". Not for scripting videos (use tt-hook-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: TikTok
---

# TikTok Profile Optimizer

You send a screenshot of your profile (or paste name, username and bio), tell me your follower count and what you want followers to do. I hand back a scorecard, a bio rewrite inside TikTok's tiny limit, which videos to pin, and the link plan.

---

## The core discovery: you have one second and about 80 characters

A viewer liked one video. They tap your name. They see your photo, name, a very short bio, three pinned videos and the top of your grid. They decide in about a second.

The question in their head: **"What will I get if I follow?"** TikTok bios are tiny (around 80 characters at the time of writing — verify), so there's room to answer exactly that and nothing else.

**Rule: the bio answers "what do I get?" The pins prove it. Cut everything else.**

---

## Step 0 — Intake

1. **Screenshot**, or name, @username, bio, link.
2. **Follower count** — the clickable link field has historically unlocked at a follower threshold (often cited as 1,000 — verify current rules and account type).
3. **Account type:** personal or business.
4. **Goal:** grow followers (default), drive signups, land clients, sell a product.
5. **Top 3–5 videos** by views or follows gained, if known.

Score only what you've been shown.

---

## Step 1 — Score the profile

| # | Part | Passes when |
|---|---|---|
| 1 | **Photo** | Clear face or clean logo, readable tiny |
| 2 | **Name** | Name + niche keyword (the name field helps search) |
| 3 | **@username** | Short, sayable, matches your other platforms |
| 4 | **Bio** | Who it's for + what they get + one specific, within the limit |
| 5 | **Link** | One goal-matched link (or a pre-unlock plan) |
| 6 | **Pinned videos** | Up to 3, each proving what following gets you |
| 7 | **Top grid** | Covers readable, clearly one niche |

---

## Step 2 — Rewrite

### Bio — who + what + one specific
1. **Lead with what a follower gets.**
   - Bad → "✨ Just a girl with big dreams ✨ | 🇬🇧 | Biz inquiries ⬇️"
   - Good → "Bookkeeping for small businesses\nOne money mistake fixed daily"
2. **One specific:** a cadence ("daily"), a niche ("for Etsy sellers"), a proof. Real only.
3. **Count every character** — emoji count too. Never deliver over the limit.

### Name field
`Name | Niche keyword` — e.g. "Priya | Small Biz Bookkeeper". Helps people find you in search.

### Link
- **Unlocked:** one link matched to the goal — newsletter, booking page, product, or a single link page with the goal link first.
- **Not unlocked yet:** say so plainly and offer the honest workarounds: put the link on a connected Instagram or YouTube profile and point to it; mention "newsletter in my Instagram bio" in captions sparingly; focus on followers until the field unlocks. Verify the current unlock rules and any business-account options with web search.

### Pinned videos — pick by goal
| Slot | Video | Why |
|---|---|---|
| 1 | Your best performer that still represents your niche | Proof people like it |
| 2 | A "start here" / who-this-is-for video, or Part 1 of a series | Tells new viewers what to expect |
| 3 | Goal video — offer, signup, results | Moves them to the next step |

If no "start here" video exists, script one (30–45 seconds): who you are, what you post, why follow, in that order. Hand the hook to `tt-hook-scripter`.

### Top grid
Readable cover text on recent videos, one niche at a glance. If the grid jumps between unrelated topics, recommend a consistent cover style going forward — don't delete videos without the user's decision.

---

## Worked example

**Input:** Name "priyamakesmoney". Bio "✨ living my best life ✨ | bookkeeper | collabs 📩". 640 followers. Goal: clients. Top video: "Things I'd never do again as a bookkeeper" (210k views).

**Output:**
```
NAME   before: priyamakesmoney
       after:  Priya | Small Biz Bookkeeper   (28)

BIO    before: ✨ living my best life ✨ | bookkeeper | collabs 📩
       after:  Bookkeeping for small business owners
               One money fix a day ↓                (59)

LINK   640 followers — clickable link likely not unlocked yet (verify).
       Plan: add booking link to your Instagram bio; in captions on client-relevant videos say "booking link on my Instagram"; review again at the threshold.

PINS   1. "Things I'd never do again" (210k — best proof)
       2. NEW: 30s "start here" — script via tt-hook-scripter
       3. Shoebox story Part 1 (shows the real work)
```

---

## Output format

```
GOAL: [ ] · FOLLOWERS: [n] · LINK UNLOCKED: [yes / no / unverified]

SCORECARD: | # | Part | Score | Reason |
TOP 3 FIXES: [ ]

REWRITES (copy-ready, with counts)
Name · Bio · Link plan · Pins (1–3 with reasons) · Grid note

"START HERE" SCRIPT (if needed): [outline]
LIMITS: [verified / unverified]
MISSING: [ ]
```

---

## Sibling skills

- `tt-hook-scripter` — script the "start here" video.
- `tt-content-planner` — make sure new videos match the bio's promise.
- `ig-profile-optimizer` — where the link lives before TikTok's unlocks.
- `x-profile-optimizer`, `threads-profile-optimizer` — other platforms.

---

## Pre-flight checklist

- [ ] Bio within the limit (emoji counted), answers "what do I get?"
- [ ] Name field carries a niche keyword?
- [ ] Link plan matches follower count — workaround if locked?
- [ ] Three pins chosen by job?
- [ ] No invented proof?
- [ ] Limits and unlock rules verified or labelled?
