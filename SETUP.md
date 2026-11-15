# Peak: install it as an app on your Android phone

You'll publish the files to GitHub Pages, which is free, and then install Peak from Chrome. It takes about 10 minutes, one time.

## 1. Put the files on GitHub (on your computer)
1. Unzip `peak-app.zip`. It contains 8 files.
2. Go to github.com and sign in. Click **+** (top right), then **New repository**.
   - Name: `peak`. Visibility: **Public**. Free GitHub Pages needs a public repo.
     Only the app's code is public. Your workout data never leaves your phone.
   - Click **Create repository**.
3. On the new repo page, click **uploading an existing file**. Drag in all 8 files, then click **Commit changes**.
4. Open the repo's **Settings**, then **Pages** (left sidebar).
   - Source: **Deploy from a branch**. Branch: **main**, folder **/ (root)**. Click **Save**.
5. Wait 1–2 minutes. Your app is live at:
   **https://YOUR-GITHUB-USERNAME.github.io/peak/**

## 2. Install it on your phone
1. Open that link in **Chrome** on your Android phone.
2. Tap **Install** on the prompt, or tap **⋮** and then **Install app**.
   You can also use Peak's own button under **Progress → Install Peak**.
3. Peak now has its own icon, opens full screen, appears in the app switcher, and works offline.

## 3. Bring your history over (once)
1. On your phone, open the **old** Peak on claude.ai. Go to **Progress → Settings → Back up → Copy**.
2. Open the **new** Peak app. Go to **Progress → Settings → Restore / import → Paste**, long-press to paste, then tap **Import**.
   This brings over your workouts, weigh-ins, food log and settings.

## Keep your data safe
- Your data is saved **on the phone**. Uninstalling Peak or clearing Chrome's site data erases it.
- Every couple of weeks, tap **Progress → Back up → Save file**. It saves a `.json` file to Downloads.
  To restore, use **Restore / import → File**.

## Updating the app later
1. Upload the new `index.html` to the repo, replacing the old one.
2. In `sw.js`, change `VERSION = "peak-v1"` to `"peak-v2"` (then v3, and so on) and upload it too.
3. Close and reopen Peak on the phone, twice if needed, to pick up the new version.
