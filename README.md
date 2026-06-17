# Chinese Lesson Deck 词

**Version 2.0.0**

A self-contained study app for the **Batch 01 华语** vocabulary — swipe-through flashcards in
Chinese with Thai, English, and (AI-generated) Japanese, plus quizzes, search, per-learner
profiles, and a growth companion that levels up as you study. It's one HTML file: no build step,
no server, no dependencies.

- **Content:** 105 words · 6 lessons · 5 fill-in-the-blank questions
- **Works:** offline, on phone or desktop, installable to the home screen
- **Profiles & progress:** stored locally on the device (not password-protected)

See **[USER_GUIDE.md](USER_GUIDE.md)** for how to use it and **[CHANGELOG.md](CHANGELOG.md)** for
version history.

---

## Quick start (no hosting)

Open the HTML file in any browser, or send it to a phone and open it there. Host it (below) only
if you want a shareable URL.

> **Tip:** rename the file to **`index.html`** so it serves at the root of your site
> (`yoursite.com` instead of `yoursite.com/ChineseLessonDeck.html`).

---

## Hosting (GitHub Pages)

1. Put the file in your repo as `index.html` (or keep its name).
2. **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`,
   Folder = `/ (root)`, **Save**.
3. After ~1 minute your app is live at `https://<username>.github.io/<repo>/`.

Other one-click options: **Netlify Drop** (drag the file onto app.netlify.com/drop) or
**Firebase Hosting** (`firebase deploy`). Custom domains are supported on all three — add the
domain in the host's dashboard, then add the DNS records it gives you at your registrar.

---

## Updating to a new version

Replace the existing HTML file in the repo with the new one (same filename), commit, and Pages
redeploys automatically in about a minute. Do a hard refresh if your browser shows the old version.

> Note: v2.0.0 changed how data is stored (per-profile). Progress from v1.0.0 does not carry over;
> the app starts fresh with a profile.

---

## Adding more lessons

The deck is generated from the lesson spreadsheets and embedded into the HTML. To grow it, provide
the lesson files (see the project notes for the expected columns); the data is regenerated, lessons
are auto-numbered by date, Japanese is generated for any new words, and the single HTML file is
rebuilt and re-deployed. No database to manage.

---

## Files in this project

| File | Purpose |
|------|---------|
| `ChineseLessonDeck.html` | The app (rename to `index.html` for hosting) |
| `USER_GUIDE.md` | How to use the app |
| `CHANGELOG.md` | Version history |
| `README.md` | This file — overview, hosting, updating |

---

*Built from `Batch01_Chinese_Lesson_Master_v0_2.xlsx`. Current version: 2.0.0.*
