# 🛡️ URL Risk Analyzer

A heuristic-based URL threat detection system — fully static, runs 100% in the browser.  
**No server required. No Python. Hosted free on GitHub Pages.**

## 🌐 Live Demo
Once deployed: `https://<your-username>.github.io/<repo-name>/`

---

## 🚀 How to Host on GitHub Pages (Step-by-Step)

### Step 1 — Create a GitHub Repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** icon (top right) → **"New repository"**
3. Name it something like `url-risk-analyzer`
4. Set it to **Public**
5. Click **"Create repository"**

### Step 2 — Upload the File
**Option A — Upload via GitHub website (easiest):**
1. Inside your new repo, click **"Add file"** → **"Upload files"**
2. Drag and drop `index.html` into the box
3. Scroll down and click **"Commit changes"**

**Option B — Using Git (command line):**
```bash
git clone https://github.com/<your-username>/url-risk-analyzer.git
cd url-risk-analyzer
cp /path/to/index.html .
git add index.html
git commit -m "Add URL Risk Analyzer"
git push
```

### Step 3 — Enable GitHub Pages
1. In your repository, click **"Settings"** (top menu)
2. Scroll down to the **"Pages"** section (left sidebar)
3. Under **"Source"**, select **"Deploy from a branch"**
4. Under **"Branch"**, select **`main`** and folder **`/ (root)`**
5. Click **"Save"**

### Step 4 — Visit Your Site
- GitHub will show a banner: *"Your site is live at https://..."*
- It usually takes **1–2 minutes** to go live
- Your URL will be: `https://<your-username>.github.io/url-risk-analyzer/`

---

## 📁 Project Structure
```
url-risk-analyzer/
└── index.html    ← Everything is in this single file
```

## ✨ Features
- 12 heuristic security checks (all run in-browser with JavaScript)
- Animated risk/safety meters with circular progress rings
- Threat level gauge with needle animation
- Spectrum risk bar indicator
- Detailed risk & safety factor breakdown
- Animated particle background
- Fully responsive design
- Zero backend — works offline too!

## 🔍 How It Works
The analyzer checks each URL against 12 heuristic rules:
1. Spammy/restricted keywords
2. HTTPS vs HTTP
3. Raw IP address usage
4. URL length
5. Suspicious TLDs (.tk, .xyz, etc.)
6. Excessive subdomains
7. Suspicious special characters
8. URL shortener detection
9. Number-heavy domain names
10. Hyphen abuse in domain
11. Trusted domain whitelist
12. Domain name length

Scores combine into a final risk percentage (0–100%):
- **0–19%**: ✅ SAFE
- **20–44%**: ℹ️ LOW RISK
- **45–69%**: ⚠️ MODERATE RISK
- **70–100%**: 🚫 HIGH RISK

---

> ⚠️ Heuristic-based analysis only. Always verify URLs through multiple sources.
