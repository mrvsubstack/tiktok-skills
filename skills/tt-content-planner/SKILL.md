---
name: tt-content-planner
description: "Builds a 7-day TikTok plan that fits how much you can actually film: which days get which video type, the hook and goal for each, how many trend rides vs original videos, a batch-filming schedule, and a balance check. Use this skill whenever the user says things like \"plan my TikTok week\", \"what should I post on TikTok\", \"how often should I post on TikTok\", \"give me a TikTok content calendar\", \"help me batch film\", or \"plan TikToks for my launch\". Not for scripting a single hook (use tt-hook-scripter) or deciding on one trend (use tt-trend-mapper)."
metadata:
  author: Mr V
  version: "1.0"
  group: TikTok
---

# TikTok Content Planner

You tell me your niche, your audience and how much time you have to film. I hand back a 7-day plan — every video with a type, hook and goal — plus a batch-filming schedule so the plan survives a busy week.

---

## The core discovery: the bottleneck is filming, not ideas

Most TikTok plans die on Wednesday. Not because the ideas ran out, but because each video meant setting up, filming, editing and posting from scratch, every single day.

The creators who post consistently batch: one or two filming sessions a week, several videos each, same setup, outfit changes optional.

**Rule: plan the filming sessions first, then the posting days. A plan you can't film isn't a plan.**

---

## Step 0 — Intake

1. **Niche** and what you're known for (or want to be).
2. **Audience** in one line.
3. **Filming capacity:** how many hours a week, how many sessions. Default: one 2-hour session.
4. **Posting target.** Default: 4–5 videos a week. Be honest — 3 good ones beat 7 rushed ones.
5. **Formats you can do:** talking head, screen recording, voiceover b-roll, demos, skits.
6. **Raw material:** results, questions people ask you, mistakes, behind-the-scenes moments.
7. **Any launch or promotion** this week.

---

## Step 1 — Set the mix

| Video type | Share | Job |
|---|---|---|
| **Teach** (how-to, mistakes, step by step) | 40% | Saves, search traffic |
| **Story / behind the scenes** | 25% | Follows, trust |
| **Opinion / contrarian** | 15% | Comments, shares |
| **Trend ride** (with a niche twist) | 10–20% | Reach — max 1–2 a week |
| **Offer** | max 1 a week | Sales |

Rules:
1. **Trend rides capped at 1–2 a week.** An account made only of trends has no identity.
2. **Series beat one-offs.** "Part 1/2/3" or "Day 12 of…" gives people a reason to follow. Plan at least one series slot.
3. **Every angle from real material.**
   - Bad → "Wed: Teach — productivity tips"
   - Good → "Wed: Teach — the 3 window positions (you got 4s → 7s watch time)"

---

## Step 2 — Assign hook and goal per video

| Goal | Hook types (see `tt-hook-scripter`) |
|---|---|
| Watch time | Result first · open loop |
| Shares | Contrarian · relatable/POV |
| Comments | Mistake callout · choice |
| Follows | Series ("Day n of…") |
| Saves | How-I step by step |

No hook type more than twice a week.

---

## Step 3 — Plan the batch session

Group videos by setup so you film them back to back:

```
SESSION [day, time, length]
Setup A (desk, talking head): videos 1, 3, 5 — change shirt between each
Setup B (screen recording): video 2
Setup C (outside / b-roll): video 4
Edit: [when] · Schedule: [when]
```

Rules:
1. **Same setup = same session.**
2. **Film 1–2 extra hooks per video** — you can test which opening works.
3. **Leave one slot open** for a trend that appears mid-week (only if it passes `tt-trend-mapper`).

---

## Step 4 — Balance check

- [ ] Fits the filming capacity?
- [ ] At least 2 teach videos?
- [ ] At least 1 story / behind the scenes?
- [ ] At least 1 series slot?
- [ ] Trend rides ≤2, each with a twist?
- [ ] Offer ≤1?
- [ ] No hook type more than twice?

Posting times: use the user's TikTok analytics (follower activity) if they have it. Otherwise write "check your analytics" — don't present generic times as fact. Verify any posting-frequency advice with current sources before stating it as fact.

---

## Worked example

**Input:** "Freelance bookkeeper. Audience: small business owners. One 2-hour session Sunday. 4 videos. Material: a client brought receipts in a shoebox; most clients miss quarterly tax dates; I use 3 apps daily."

**Output:**
| Day | Type | Hook | Goal | Angle | Setup |
|---|---|---|---|---|---|
| Mon | Teach | Mistake callout | Comments | "If you only think about taxes in April, you're paying late fees" | A |
| Tue | Story | Result first | Follows | "A client brought me 14 months of receipts in a shoebox. Day 1:" (Part 1) | A |
| Thu | Teach | How-I | Saves | "The 3 apps I open every morning" | B |
| Sat | Trend ride | (via tt-trend-mapper) | Shares | "Things I'd never do again as a bookkeeper" | A |

SESSION: Sunday 10–12 · Setup A: Mon, Tue, Sat back to back · Setup B (screen record): Thu · Edit Sunday afternoon.
Series: shoebox story Part 2 next week.

---

## Output format

```
WEEK OF [date] · Niche: [ ] · Capacity: [sessions/hours] · Videos: [n]
Mix: Teach [ ] · Story [ ] · Opinion [ ] · Trend [ ] · Offer [ ]

| Day | Type | Hook | Goal | Angle (source) | Setup |

BATCH SESSION: [setup groups, extra hooks to film, edit/schedule time]
SERIES: [what continues next week]
OPEN SLOT: [for a mid-week trend, if any]
BALANCE CHECK: [✓/✗]
MISSING MATERIAL: [ ]
```

---

## Sibling skills

- `tt-hook-scripter` — script each opening.
- `tt-caption-writer` — caption each video.
- `tt-trend-mapper` — vet the trend slot.
- `tt-profile-optimizer` — new viewers check your profile before following.
- `ig-content-planner` — if the same videos go to Reels.

---

## Pre-flight checklist

- [ ] Filming sessions planned before posting days?
- [ ] Plan fits the user's real capacity?
- [ ] Every angle from real material?
- [ ] Trend rides capped, series slot included?
- [ ] Balance check run?
- [ ] Timing advice from analytics or labelled?
