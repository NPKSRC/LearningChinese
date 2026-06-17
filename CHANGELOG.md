# Changelog

All notable changes to **Chinese Lesson Deck** are recorded here.
Format follows [Keep a Changelog](https://keepachangelog.com/); versions follow
[Semantic Versioning](https://semver.org/): **MAJOR.MINOR.PATCH**.

---

## [2.0.0] — 2026-06-17

A major update that turns the app from a single-user flashcard tool into a personalized,
gamified study companion. Built from `Batch01_Chinese_Lesson_Master_v0_2.xlsx`.

### Added
- **Local learner profiles** — create a profile with a name and a chosen companion; switch or add
  profiles from the Me tab. Each profile keeps its own progress, settings, and growth, saved on
  the device. (No password / no cross-device sync — see Notes.)
- **Growth companion** — pick a **dragon, phoenix, or warrior** that evolves through five stages
  (Egg → Hatchling → Young → Grown → Legendary) as you earn XP, with an evolution celebration.
- **XP & daily streak** — XP from viewing words, answering quiz questions, and a daily-return
  bonus that builds a 🔥 streak. New **Me** tab shows the mascot, stage, XP bar, streak, and stats.
- **Japanese translations (AI-generated)** for all 105 words, clearly marked with an **AI** badge.
- **Per-card language checkboxes** — toggle Pinyin / Thai / English / Japanese independently on
  the card back; selection is remembered.
- **Quiz "Skip"** — defer a question to the end of the quiz; skipping doesn't affect accuracy.
- **Quiz direction toggle** — practice 中→ไทย or ไทย→中.

### Changed
- **Serialized lessons** — the UI now shows "Lesson 1–6" (and "L1–L6" in Browse) instead of the
  raw dates; the original dates are kept in the data behind the scenes.
- **Study navigation** redesigned around free left/right **swiping** (plus arrows and keyboard),
  with **tap to flip**; the difficulty buttons became **optional tags** decoupled from navigation.
- The 4th tab is now **Me** (growth + stats + profiles), replacing the old Stats tab.

### Fixed
- **Quiz layout no longer jumps** between questions — the question card and answer area now reserve
  a stable minimum height.

### Notes
- Profiles and progress are stored locally per device and are not secured by a password.
- Because storage now uses the new profile structure, progress from v1.0.0 does not carry over;
  the app starts fresh with a profile on first launch of this version.

---

## [1.0.0] — 2026-06-17

First public release (live on GitHub Pages).

### Added
- Flashcards (tap to flip), multiple-choice and fill-in-the-blank quizzes, searchable Browse,
  Stats, Chinese text-to-speech audio, lesson filtering, and a Chinese ⇄ Thai direction toggle.
- Offline-capable, installable single HTML file with progress saved on the device.

### Content
- 105 vocabulary items (39 with example sentences) and 5 fill-in-the-blank questions across 6
  lessons.

---

## Planned

Ideas under consideration (not yet committed):

### [Unreleased]
- **More lesson batches** merged into the combined deck (auto-numbered by date).
- **Real accounts with cloud sync** (e.g. Firebase) so a profile follows a learner across devices.
- **Listening mode** — hear a word and recall it before revealing the text.
- **Dedicated sentence-study mode** using the full example-sentence bank.
- **Export / import progress** between devices.
- **Light/dark theme** toggle.

---

[2.0.0]: this release
[1.0.0]: first public release
