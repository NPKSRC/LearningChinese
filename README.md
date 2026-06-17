# Chinese Lesson Deck 词

A self-contained study app for the **Batch 01 华语** vocabulary — flashcards with spaced
repetition, quizzes, search, and progress tracking, in **Chinese ⇄ ไทย**. It's one HTML
file with no build step, no server, and no dependencies to install.

- **Content:** 105 words · 6 lessons · 5 fill-in-the-blank questions
- **Works:** offline, on phone or desktop, installable to the home screen
- **Privacy:** all progress stays on the user's device

See **[USER_GUIDE.md](USER_GUIDE.md)** for how to use it and **[CHANGELOG.md](CHANGELOG.md)**
for version history.

---

## Quick start (no hosting)

Just open `ChineseLessonDeck.html` in any browser, or send the file to a phone and open it
there. That's enough for personal use. Host it (below) only if you want a shareable URL or
your own domain.

> **Tip:** before hosting, rename the file to **`index.html`**. Web hosts serve `index.html`
> automatically at the root of your site, so your URL becomes `yoursite.com` instead of
> `yoursite.com/ChineseLessonDeck.html`.

---

## Hosting options

This is a static site (one HTML file), so hosting is quick and free. Three good paths,
easiest first.

### Option A — Netlify Drop (fastest, no account or tools)
1. Rename the file to `index.html`.
2. Go to **app.netlify.com/drop**.
3. Drag the file onto the page.
4. You get a live `https://random-name.netlify.app` URL immediately.
5. (Optional) Create a free account to keep the site, rename it, or add a custom domain.

### Option B — GitHub Pages (good if you want version control)
1. Create a GitHub repository.
2. Add the file as `index.html` (commit and push, or upload via the web UI).
3. In the repo: **Settings → Pages**.
4. Under **Build and deployment**, set **Source = Deploy from a branch**, **Branch = main**,
   **Folder = / (root)**, then **Save**.
5. After a minute your app is at `https://<username>.github.io/<repo>/`.

### Option C — Google Firebase Hosting (Google's static-hosting tool)
Firebase is Google's recommended way to host a static site. You'll need
[Node.js](https://nodejs.org) installed.

1. Install the CLI:
   ```bash
   npm install -g firebase-tools
   ```
2. Sign in with your Google account:
   ```bash
   firebase login
   ```
3. Put `index.html` in an empty folder, open a terminal there, and run:
   ```bash
   firebase init hosting
   ```
   When prompted:
   - **Create / select a project** (e.g. `chinese-lesson-deck`).
   - **Public directory:** enter `.` (a dot — the current folder) **or** put your file in a
     `public/` folder and accept the default.
   - **Single-page app rewrite to /index.html?** → **No**.
   - **Set up automatic builds with GitHub?** → **No** (not needed).
   - If it asks to overwrite `index.html`, choose **No**.
4. Deploy:
   ```bash
   firebase deploy
   ```
5. Your app is live at `https://<project-id>.web.app`.

> **About Google Sites / Google Drive:** Google Sites can't host a raw interactive HTML/JS
> app at its own URL — it can only *embed* one via an iframe. Google Drive no longer serves
> hosted HTML either. For a Google-native solution, use **Firebase Hosting** (above) or
> **Google Cloud Storage** static website hosting. Firebase is much simpler for this.

---

## Using your own domain

All three hosts above support custom domains with free automatic HTTPS. The pattern is the
same everywhere:

1. **In the host's dashboard**, add your domain (e.g. Netlify: *Domain settings → Add a
   domain*; Firebase: *Hosting → Add custom domain*; GitHub Pages: *Settings → Pages →
   Custom domain*).
2. **At your domain registrar** (where you bought the domain — GoDaddy, Namecheap, Google
   Domains/Squarespace, Cloudflare, etc.), add the DNS records the host gives you. Typically:
   - A **CNAME** record for `www` pointing to the host's address, and/or
   - **A / AAAA** records (or a CNAME) for the apex/root domain.
3. **Wait for DNS to propagate** (minutes to a few hours). The host then issues an HTTPS
   certificate automatically.

The exact records are provided by your host during step 1 — follow those, since they differ
slightly per provider.

---

## Updating the app later

When more lesson batches are ready, the data is regenerated from the Excel files and embedded
back into the single HTML file, then re-deployed (drag a new file to Netlify, push to GitHub,
or `firebase deploy` again). No database or backend to manage.

---

## Files in this project

| File | Purpose |
|------|---------|
| `ChineseLessonDeck.html` | The app (rename to `index.html` for hosting) |
| `USER_GUIDE.md` | How to use the app |
| `CHANGELOG.md` | Version history |
| `README.md` | This file — overview and hosting |

---

*Built from `Batch01_Chinese_Lesson_Master_v0_2.xlsx`. Current version: 0.1.0.*
