# Iron Log — put it online with GitHub Pages

This turns your app into a real installable app on your phone: a proper
icon, opens in its own window (no browser bar), and works offline.

## 1. Create the GitHub repo

1. Go to github.com and sign in (create a free account if you don't have one).
2. Click **+** (top right) → **New repository**.
3. Name it something like `iron-log`. Keep it **Public** (required for free
   GitHub Pages). Don't add a README here — you already have one.
4. Click **Create repository**.

## 2. Upload the files

On the new repo's page:

1. Click **Add file** → **Upload files**.
2. Drag in everything from this folder, keeping the structure:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `apple-touch-icon.png`
   - `icons/icon-192.png`
   - `icons/icon-512.png`
3. Scroll down, click **Commit changes**.

(If you're comfortable with git instead of the web UI: `git init`,
`git add .`, `git commit -m "Iron Log"`, add your GitHub repo as the
remote, `git push`.)

## 3. Turn on GitHub Pages

1. In the repo, go to **Settings** → **Pages** (left sidebar).
2. Under **Build and deployment** → **Source**, choose **Deploy from a
   branch**.
3. Branch: `main`, folder: `/ (root)`. Click **Save**.
4. Wait ~1 minute, then refresh — GitHub will show your live URL:
   `https://<your-username>.github.io/iron-log/`

## 4. Install it on your phone

- **iPhone (Safari):** open that URL → Share icon → **Add to Home Screen**.
- **Android (Chrome):** open that URL → ⋮ menu → **Add to Home screen** /
  **Install app**.

It'll now have its own icon, open full-screen with no browser bar, and
keep working even with no signal.

## Updating it later

Any time you want to change the app: edit `index.html` on GitHub (or
upload a new version the same way), commit, and it goes live within a
minute or two. Your gym data itself isn't affected — it lives in the
browser storage on your phone, separate from the code.

## About your data

- Your workout data lives in the app's local storage on your phone —
  it does **not** get uploaded to GitHub. GitHub only hosts the code.
- Use the **Backup to file** button inside the app regularly and save
  that file somewhere (Drive, email to yourself, etc.) as your actual
  data backup.
