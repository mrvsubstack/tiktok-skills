---
name: tt-caption-writer
description: "Writes the caption and on-screen text plan for a finished TikTok: a first line that gives viewers a reason to comment or keep watching, search keywords people actually type, a small mixed hashtag set, and a settings checklist (comments, duet, stitch, branded content). Delivered copy-ready to paste when you upload. Use this skill whenever the user says things like \"write my TikTok caption\", \"what hashtags for this TikTok\", \"caption this video\", \"what text should I put on screen\", \"make people comment on my TikTok\", or \"TikTok SEO for this video\". Not for the spoken hook in the first 2 seconds (use tt-hook-scripter)."
metadata:
  author: Mr V
  version: "1.0"
  group: TikTok
---

# TikTok Caption Writer

You tell me what the video is, what it says and what you want viewers to do. I hand back a caption, a keyword list, 3–5 hashtags, an on-screen text plan and an upload settings checklist.

---

## The core discovery: on TikTok the caption is a search box and a comment starter

Nobody watches a TikTok for its caption. But the caption does two jobs the video can't:

1. **Search.** More and more people search TikTok like a search engine. The words in your caption and on-screen text help TikTok understand what the video answers.
2. **Comments.** A caption that asks something specific turns watchers into commenters, and comments keep the video alive.

**Rule: the caption names what the video is about in the words people search, then gives them one specific reason to comment.**

---

## Step 0 — Intake

1. **What the video is about**, and the spoken hook if it's scripted.
2. **Goal:** comments (default), watch time, shares, follows, saves.
3. **Audience** in one line.
4. **Is it promotional, sponsored or affiliate?** This changes the disclosure settings.
5. **Sound:** original audio or a trending sound (credit it).

---

## Step 1 — Find the search keywords

List 3–5 phrases someone would type to find this video:
- Bad → "content", "tips", "creator life"
- Good → "how to light videos at home", "window lighting tiktok", "cheap filming setup"

Use web search or TikTok's own search suggestions to check what people actually type. Label the list as checked or unchecked.

Put the top keyword phrase **naturally** in the first line of the caption and in the on-screen text.

---

## Step 2 — Write the caption

1. **First line: keyword + reason to engage.** Most viewers only see a line or two.
   - Bad → "New video!! 🔥🔥"
   - Good → "Window lighting for videos — which spot works in your room? 1, 2 or 3?"
2. **Short.** One to three lines usually beats a paragraph. TikTok allows long captions (thousands of characters — verify the current limit), but long rarely helps unless it's a mini-tutorial people will save.
3. **One comment trigger:**
   | Trigger | Example |
   |---|---|
   | Choice | "1, 2 or 3 — which are you trying first?" |
   | Your version | "What's the cheapest thing that improved your videos?" |
   | Part 2 bait (honest) | "Part 2 is the editing settings — want it?" (only if you'll make it) |
   | Fill the gap | "I left out one spot on purpose. Guess which." |
4. **No engagement bait** — "comment 'YES' for the link", "like if you agree".
5. **0–2 emoji.**

---

## Step 3 — Hashtags

**3–5 tags, mixed:**
- 2–3 **niche** tags (specific, the community).
- 1–2 **topic** tags (broader subject).
- 0–1 **broad** tag.

Every tag describes the video. No #fyp walls — they don't describe anything. Tell the user to check tag sizes in the app's search.

---

## Step 4 — On-screen text plan

Text on the video is read by viewers **and** helps TikTok understand the topic.
1. **Hook text** (first second) — from `tt-hook-scripter` if scripted.
2. **Step labels** — "1. Face the window", "2. 45 degrees", "3. Behind the camera".
3. **Keyword** — include the main search phrase once, naturally.
4. **Safe zone** — keep text away from the bottom caption area and the right-side buttons.

---

## Step 5 — Upload settings checklist

Check these when uploading (names change — verify in the app):
- [ ] **Who can view:** everyone (unless testing).
- [ ] **Comments:** on.
- [ ] **Duet / Stitch:** on if you want remixes (often good for reach), off for sensitive content.
- [ ] **Disclose commercial content / branded content / paid partnership:** **on** if the video promotes your own business, a brand deal or an affiliate link. This is a rule, not a preference — check current TikTok policy and your country's ad disclosure law.
- [ ] **Sound credited** if it's not original.
- [ ] **AI-generated content label** on, if any part is AI-generated and realistic (check current policy).

---

## Worked example

**Input:** "Video: 3 window positions for lighting, talking head. Goal: comments. Audience: new creators. Not sponsored. Original audio."

**Output:**
```
--- CAPTION (copy-ready) ---
Window lighting for videos at home — which spot fits your room, 1, 2 or 3?
#windowlighting #smallcreatortips #filmingsetup #contentcreatortips
--- END ---

KEYWORDS: window lighting for videos · how to light videos at home · cheap filming setup (unchecked — confirm in TikTok search)
ON-SCREEN: 0–1s "No new gear" · step labels "1. Face it" "2. 45°" "3. Behind camera" · keyword in the step-1 label
SETTINGS: everyone · comments on · duet/stitch on · commercial content OFF (not promotional) · original audio
```

---

## Output format

```
GOAL: [ ] · PROMO/SPONSORED: [yes/no]

--- CAPTION (copy-ready) ---
[caption]
[hashtags]
--- END ---

KEYWORDS: [phrases] (checked / unchecked)
ON-SCREEN TEXT PLAN: [timestamps → text]
SETTINGS CHECKLIST: [each item with recommended state]
Characters: [n]
```

---

## Sibling skills

- `tt-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `tt-hook-scripter` — the spoken and visual hook.
- `tt-trend-mapper` — if it rides a trend, credit the sound.
- `tt-content-planner` — where this video sits in the week.
- `ig-caption-writer` — cross-posting the same video as a Reel needs a different caption.

---

## Pre-flight checklist

- [ ] Search keywords listed and placed in the first line and on-screen?
- [ ] One specific comment trigger, no bait?
- [ ] 3–5 descriptive hashtags, no #fyp wall?
- [ ] On-screen text in the safe zone?
- [ ] Commercial disclosure set correctly for promo content?
- [ ] Limits and setting names verified or labelled?
