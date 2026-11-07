---
name: tt-hook-scripter
description: "Scripts the first 2 seconds of a TikTok (or Reel/Short): the spoken line, the on-screen text and the opening visual, built as three layers that each stop the scroll on their own — plus the next 3–5 seconds that keep people watching. Gives 3 hook options picked by the video's goal. Use this skill whenever the user says things like \"write a TikTok hook\", \"how should I open this video\", \"my TikToks die in the first second\", \"give me hooks for this video\", \"script the opening\", or \"what should I say first on camera\". Not for the caption under the video (use tt-caption-writer) or riding a trending sound (use tt-trend-mapper)."
metadata:
  author: Mr V
  version: "1.0"
  group: TikTok
---

# TikTok Hook Scripter

You tell me what the video is about, what's in it, and what you want viewers to do. I hand back 3 opening scripts — each with the spoken line, the on-screen text and the first visual — plus a beat sheet for the seconds after.

---

## The core discovery: a hook is three hooks at once

People watch TikTok with sound off, with sound on, and while half looking. So the first 2 seconds need three layers, and **each layer must work alone**:

1. **Visual** — what's moving or surprising in frame 1, before anyone reads or listens.
2. **On-screen text** — for sound-off viewers. Big, short, readable in a second.
3. **Spoken line** — for sound-on viewers. The first words, not a "Hey guys".

Most weak hooks have one layer and two blanks: a talking head saying "So today I want to talk about…" with no text and no movement.

**Rule: script all three layers for every hook. If any layer is empty or just repeats another word for word, it's not finished.**

---

## Step 0 — Intake

1. **What the video is about** and what actually happens in it.
2. **The payoff** — what the viewer gets by the end.
3. **Goal:** watch time (default), shares, comments, follows, saves.
4. **Format:** talking head, screen recording, voiceover on b-roll, demo, skit.
5. **What you can film** — be realistic. Don't script a drone shot for a phone creator.
6. **Any real result or number.** Never invented.

---

## Step 1 — Pick the hook type by goal

| Goal | Hook | Spoken line shape | Visual |
|---|---|---|---|
| **Watch time** | Result first | "This [result] took me [time]." | Show the result in frame 1 |
| | Open loop | "Number 3 is the one nobody does." | Hand counting, list on screen |
| **Shares** | Contrarian | "Stop [common advice]. Here's why." | You doing the "wrong" thing |
| | "POV" / relatable | A shared moment, acted out | The moment itself, no intro |
| **Comments** | Mistake callout | "If you [common habit], you're losing [thing]." | The habit on screen |
| | Choice | "Which one would you pick?" | Two options side by side |
| **Follows** | Series | "Day [n] of [challenge]." | Progress shot |
| **Saves** | How-I | "How I [result] in [time] — step by step." | Screen or process already moving |

Give 3 options on different hooks. Recommend one.

---

## Step 2 — Write each layer

### Visual (frame 1)
1. **Motion or surprise in the first frame.** Not a static face waiting to speak.
   - Bad → You, centred, smiling, saying "Hey guys".
   - Good → Your hand dropping a $40 ring light into a bin.
2. **Start mid-action.** Cut the first second of any clip where nothing happens.

### On-screen text
1. **Under ~8 words.** Readable in one second.
2. **Not a transcript of the spoken line.** It should add or sharpen.
   - Spoken: "This is the only light I use now." / Text: "Stop buying gear."
3. **Placed in the safe zone** — away from the bottom caption area and the right-side buttons.

### Spoken line
1. **The first words are the hook.** No "Hey guys", "So", "Okay so", "In this video".
2. **Under ~2 seconds to say.** Read it out loud and time it.
3. **Sayable.** Short words. Contractions. No written-English sentences.
   - Bad → "In today's video I'm going to be discussing the importance of lighting."
   - Good → "This window is better than a $200 light."

---

## Step 3 — Script the next 3–5 seconds

The hook buys 2 seconds. The next beat buys the rest.
1. **Pay off a piece of the promise fast** — show the first step or the first proof.
2. **Keep a loop open** — "but the third one is the one that matters".
3. **Cut every 1–3 seconds** in talking-head videos (verify current advice for your niche — some audiences prefer long single takes).

---

## Step 4 — Make sure it's honest

The payoff must be in the video. A hook that promises something the video doesn't deliver gets swiped and teaches viewers to skip you. If the result is a number, it's the user's real number.

---

## Worked example

**Input:** "Video: how I light my videos with just a window. Payoff: 3 positions to try. Goal: saves. Format: talking head + quick cuts. Result: average watch time went from 4s to 7s after switching."

**Output:**
```
A) How-I  ← recommended (goal = saves)
Visual:   Fast cut from a dim, grainy shot to the bright window-lit shot of the same face
Text:     "4s → 7s watch time. No new gear."
Spoken:   "I fixed my lighting for free. Three spots — the last one's the best."
Next 3–5s: Point to the window, step into position 1, on-screen "1. Face the window"

B) Contrarian
Visual:   Ring light dropped into a bin
Text:     "Stop buying gear."
Spoken:   "This window beats every light I've bought."

C) Mistake callout
Visual:   Side-lit shot with a harsh shadow down the face
Text:     "This is why you look tired on camera"
Spoken:   "If your window's beside you, you're half in shadow."
```

---

## Output format

```
VIDEO: [one line] · GOAL: [ ] · FORMAT: [ ]

A) [hook type] ← recommended
Visual:     [frame 1]
Text:       [on-screen, ≤8 words]
Spoken:     [first line, ≤2s]
Next 3–5s:  [beat]
Why:        [one line]

B) …   C) …

FILMING NOTES: [cuts, angle, where text sits]
Placeholders to fill: [ ]
Next: caption it with tt-caption-writer.
```

---

## Sibling skills

- `tt-caption-writer` — caption, hashtags and settings for the finished video.
- `tt-trend-mapper` — the hook is a trend ride.
- `tt-content-planner` — fit this video into the week.
- `ig-hook-extractor` — break down a Reel you admire first.
- `killer-scripter` — write the full video script beyond the hook.

---

## Pre-flight checklist

- [ ] All three layers scripted, none duplicating another word for word?
- [ ] Frame 1 has motion or surprise?
- [ ] Spoken line starts with the hook, under ~2 seconds?
- [ ] On-screen text under ~8 words, in the safe zone?
- [ ] Next 3–5 seconds pay off a piece of the promise?
- [ ] Payoff actually in the video, numbers real?
