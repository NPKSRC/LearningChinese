# Changelog

All notable changes to **Chinese Lesson Deck** are recorded here.
Format follows [Keep a Changelog](https://keepachangelog.com/); versions follow
[Semantic Versioning](https://semver.org/) (MAJOR.MINOR.PATCH).

---

## [0.1.0] — 2026-06-17

First working release. Built from a single source file,
`Batch01_Chinese_Lesson_Master_v0_2.xlsx` (schema v0.2, Batch 01).

### Added
- **Study mode** with spaced-repetition flashcards (simplified SM-2 scheduling):
  Again / Hard / Good / Easy ratings, per-word intervals, and a session queue of
  due cards plus new cards.
- **Tap-to-flip cards** showing 汉字 on the front; Pinyin, Thai meaning, English gloss,
  and an example sentence (when available) on the back.
- **Quiz mode** combining auto-generated multiple-choice questions with the 5 original
  fill-in-the-blank warm-up questions (A/B/C choices + Thai hint).
- **Browse mode** — searchable list of all 105 words (matches 汉字 / Pinyin / Thai /
  English), with tap-to-hear audio.
- **Stats** — words started, words mastered (7+ day interval), words due, and lifetime
  quiz accuracy.
- **Direction toggle** — 中→ไทย and ไทย→中 for both study and quiz.
- **Lesson filter** — study/quiz All or a single lesson (8.10, 8.17, 8.24, 9.07, 9.21, 9.28).
- **Audio** — Chinese text-to-speech via the device's built-in voice.
- **Offline-capable, installable** single HTML file; "Add to Home Screen" for an app-like
  experience.
- **Progress persistence** with a layered storage approach
  (window.storage → localStorage → in-memory fallback).

### Content
- 105 vocabulary items across 6 lessons; 39 items include example sentences.
- 5 fill-in-the-blank questions.

### Known limitations
- Thai translations of example sentences were absent in this batch, so example
  sentences display Chinese + Pinyin only.
- Audio depends on a Chinese voice being installed on the device; absent that, the
  speaker button is silent.
- Progress is per-device and not synced across browsers or phones.

---

## Planned

Ideas under consideration for future versions (not yet committed):

### [Unreleased]
- **Merge all lesson batches** (10+ files) into one combined deck with a batch/lesson filter.
- **Listening mode** — hear a word and recall it before revealing the text.
- **Dedicated sentence-study mode** using the full example-sentence bank.
- **Daily review reminder** / streak tracking.
- **Export / import progress** so study history can move between devices.
- **Light/dark theme** toggle.

---

[0.1.0]: initial release
