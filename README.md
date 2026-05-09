# 📱 Call Soundboard

A Progressive Web App that plays sounds during calls — crickets on silence, custom sounds when trigger words are spoken.

## Features
- 🦗 Silence detection with configurable timeout
- 🎯 Custom phrase triggers (e.g. "mother in law" → Imperial March)
- 🎸 10 built-in sounds
- ➕ Add unlimited custom triggers
- 📱 Installable as a home screen app (PWA)

---

## 🚀 Deploy to GitHub Pages (3 steps)

### Step 1 — Create a new GitHub repo
1. Go to [github.com/new](https://github.com/new)
2. Name it `call-soundboard`
3. Set it to **Public**
4. Click **Create repository**

### Step 2 — Upload these files
**Option A — Drag & drop (easiest):**
1. On your new repo page, click **uploading an existing file**
2. Drag the entire `call-soundboard` folder contents into the page
3. Click **Commit changes**

**Option B — GitHub CLI:**
```bash
cd call-soundboard
git init
git add .
git commit -m "Initial commit"
gh repo create call-soundboard --public --push --source=.
```

**Option C — Git:**
```bash
cd call-soundboard
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/call-soundboard.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. In your repo, go to **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose branch: **main**, folder: **/ (root)**
4. Click **Save**

⏱️ Wait ~60 seconds, then your app is live at:
```
https://YOUR_USERNAME.github.io/call-soundboard/
```

---

## 📲 Install on iPhone
1. Open the URL above in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button (box with arrow)
3. Tap **Add to Home Screen**
4. Tap **Add**

It will appear on your home screen and open fullscreen like a native app!

---

## 📲 Install on Android
1. Open the URL in **Chrome**
2. Tap the **⋮ menu**
3. Tap **Add to Home Screen** or **Install App**

---

## Usage
- Tap **▶ LISTEN** and allow microphone access
- The app listens during your call
- Silence for the set duration → plays your silence sound
- Say a trigger phrase → plays the matched sound
- Tap **▶ test** on any card to preview sounds

---

## Notes
- The app listens via your device microphone, so it picks up what you say (not the other person)
- Works best on a second device placed nearby during the call
- Sounds have a 4-second cooldown to prevent stacking
- All settings reset on page refresh (no server needed — everything runs locally)
