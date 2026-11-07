---
name: tt-trend-mapper
description: "Decides whether a trending TikTok sound or format fits your niche — ride it, bend it, or skip it — then scripts the twist that makes it yours: the recognisable beat first, your niche's turn second. Uses web search to check what's trending when available, and never fakes a trend's popularity. Use this skill whenever the user says things like \"should I do this trend\", \"make this TikTok trend fit my niche\", \"what trends can I use this week\", \"is this sound still trending\", \"my trend videos feel cringe\", or \"find trends for my niche\". Not for writing a hook from scratch (use tt-hook-scripter) or planning the week (use tt-content-planner)."
metadata:
  author: Mr V
  version: "1.0"
  group: TikTok
---

# TikTok Trend Mapper

You bring a trend — a sound, a format, a link to an example — or ask what's trending in your niche. I hand back a verdict (**ride / bend / skip**), the trend's native structure, and a scripted twist that makes it yours.

---

## The core discovery: the twist is the whole point

A trend gives you two things for free: a sound people recognise and a format they already know how to watch. That's a head start, not a video.

Copy the trend straight and you're the 40,000th version. Force it onto a niche it doesn't fit and your audience cringes. The videos that work hit the **recognisable beat** in the first second, then **turn it into something only your niche would make**.

And saying no is a feature. A skipped trend costs nothing. A forced one costs trust.

**Rule: no twist, no ride.**

---

## Step 0 — Intake

1. **The trend:** sound name, format description, or an example video (describe it — I can't watch links).
2. **Your niche** and what you usually post.
3. **How often you've seen it** in your feed and over what time — this is the best saturation signal you have.
4. **What you can film** this week.

If the user asks "what's trending?": use web search for current TikTok trend roundups and TikTok's Creative Center (if accessible) and say where each trend came from and when. If you can't verify a trend is current, say so. Never claim a trend is rising without a source or the user's own observation.

---

## Step 1 — The fit check

A trend must clear all four:

| # | Question | Fail looks like |
|---|---|---|
| 1 | **Niche fit:** can your audience tell why *you* did this? | The only link is "it was trending" |
| 2 | **Timing:** is it still early? | It's on every third video you see |
| 3 | **Native structure:** can you honour the expected beat? | You'd have to ignore the cut or punchline to make it work |
| 4 | **Twist:** can you say something only your niche would say? | Your version is just the trend with your face |

**Verdict:**
- **Ride** — passes all four.
- **Bend** — passes 1, 3, 4 but timing is late: only ride with a twist strong enough to work without the trend's lift, or subvert it (do the opposite).
- **Skip** — fails niche fit or twist. Explain why in one line.

---

## Step 2 — Read the lifecycle

| Stage | Signs | Move |
|---|---|---|
| **Emerging** | A few breakout videos, climbing fast | Ride now |
| **Peaking** | Everywhere, big accounts on it | Ride only with a strong twist |
| **Saturated** | Joke is worn, every third video | Skip or subvert |
| **Dead** | Stopped climbing days ago | Skip |

Base the stage on what the user has seen and what web search shows, and label it as an estimate.

---

## Step 3 — Tear down the native structure

Name exactly what the trend expects:
- **The beat** — where the drop or cut lands.
- **The setup** — the line or situation that starts it.
- **The joke or payoff** — where the reveal goes.
- **The visual convention** — pointing at text, outfit change, transition, etc.

---

## Step 4 — Script the twist

Shape: `[trend's expected setup] — but for [your niche]`.

1. **First second reads as the trend.** Same sound, same setup, same framing.
2. **Turn on the beat.** The niche twist lands exactly where the trend's payoff normally lands.
3. **Keep the native cut and timing.**
4. **Script all three layers** (visual, on-screen text, spoken line if any) — see `tt-hook-scripter`.

Rules:
1. **Never punch down** or mock the original creator.
2. **Credit the sound** and use it only if it's available for your account type — business accounts often have a restricted commercial library. Tell the user to check.
3. **Never fake popularity.**

---

## Worked example

**Input:** "Trend: the 'things I'd never do again' format with a soft piano sound — creator lists 3 things with a text overlay each, deadpan face. I've seen it maybe 10 times this week. Niche: freelance bookkeeping."

**Output:**
```
VERDICT: RIDE
FIT: 1 ✓ (bookkeepers have very specific "never again" pain) · 2 ✓ (seen ~10x this week — estimate: emerging/peaking) · 3 ✓ (simple structure) · 4 ✓ (niche-only twist available)

NATIVE STRUCTURE: deadpan face · soft piano · 3 text overlays, one per beat · no talking

TWIST SCRIPT
0–1s   Deadpan to camera, laptop open · Text: "Things I'd never do again as a bookkeeper"
Beat 1 Text: "Take a client who says 'it's all in a shoebox'"
Beat 2 Text: "Reconcile 14 months the night before the deadline"
Beat 3 Text: "Say 'quick question' is ever quick"
End    Hold deadpan, slow sip of coffee

SOUND: credit it; check it's available for your account type
CAPTION → tt-caption-writer · keyword: "bookkeeper life"
```

---

## Output format

```
TREND: [ ] · SOURCE: [user observation / web search link + date]
VERDICT: [ride / bend / skip] — [one-line reason]
FIT CHECK: 1 [✓/✗] · 2 [✓/✗] · 3 [✓/✗] · 4 [✓/✗]
LIFECYCLE: [stage] (estimate)
NATIVE STRUCTURE: [beat / setup / payoff / visual convention]
TWIST SCRIPT: [timestamped layers]
SOUND NOTE: [credit + availability check]
NEXT: tt-caption-writer
```

---

## Sibling skills

- `tt-hook-scripter` — hooks that don't depend on a trend.
- `tt-caption-writer` — caption and sound credit.
- `tt-content-planner` — one trend ride a week is usually plenty.
- `content-ideation` — when you need original ideas, not trends.

---

## Pre-flight checklist

- [ ] All four fit questions answered?
- [ ] Verdict given — skip recommended when fit fails?
- [ ] Lifecycle labelled as an estimate with its source?
- [ ] Native structure named and honoured?
- [ ] Twist lands on the trend's beat?
- [ ] Sound credit and availability noted?
- [ ] No faked popularity?
