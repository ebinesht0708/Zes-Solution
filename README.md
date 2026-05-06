# Zes Solutions Website

Official website for **Zes Solutions** — Digital Automation & Marketing Agency, Chennai.

## 🚀 Deploy to Hostinger via GitHub

Follow the steps below to host this website on Hostinger using GitHub auto-deployment.

---

## 📁 File Structure

```
zes-website/
├── index.html                        ← Main website file
├── .github/
│   └── workflows/
│       └── deploy.yml                ← Auto-deploy workflow
└── README.md
```

---

## ✅ Step-by-Step Deployment Guide

### STEP 1 — Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click the **+** icon → **New repository**
3. Name it: `zes-solutions-website`
4. Set it to **Private** (recommended) or Public
5. Click **Create repository**

---

### STEP 2 — Upload Files to GitHub

#### Option A — Using GitHub Website (Easiest)

1. Open your new repository on GitHub
2. Click **Add file** → **Upload files**
3. Drag and drop the entire `zes-website` folder contents:
   - `index.html`
   - `.github/` folder (with `workflows/deploy.yml` inside)
   - `README.md`
4. Scroll down → Click **Commit changes**

#### Option B — Using Git (Terminal/Command Prompt)

```bash
# 1. Install Git from https://git-scm.com if you haven't
# 2. Open terminal/command prompt and run:

git clone https://github.com/YOUR_USERNAME/zes-solutions-website.git
cd zes-solutions-website

# Copy your files into this folder, then:
git add .
git commit -m "Initial website upload"
git push origin main
```

---

### STEP 3 — Get Your Hostinger FTP Details

1. Log in to [hostinger.com](https://hostinger.com)
2. Go to **hPanel** (your hosting dashboard)
3. Click on **Hosting** → Select your plan
4. In the left menu, click **Files** → **FTP Accounts**
5. Note down these 3 details:
   - **FTP Server** (looks like: `ftp.yourdomain.com`)
   - **FTP Username** (usually your email or a generated username)
   - **FTP Password** (set one if not already set)

> 💡 Tip: The FTP Server is sometimes listed as your domain name or an IP. Check under "FTP Accounts" details.

---

### STEP 4 — Add FTP Secrets to GitHub

This is how GitHub securely stores your Hostinger login without exposing it publicly.

1. Go to your GitHub repository
2. Click **Settings** (top tab)
3. In left sidebar → Click **Secrets and variables** → **Actions**
4. Click **New repository secret** and add these 3 secrets:

| Secret Name    | Value (from Step 3)               |
|----------------|-----------------------------------|
| `FTP_SERVER`   | Your FTP server (e.g. `ftp.zessolutions.in`) |
| `FTP_USERNAME` | Your FTP username                 |
| `FTP_PASSWORD` | Your FTP password                 |

---

### STEP 5 — Trigger the First Deployment

1. Go back to your repository on GitHub
2. Click the **Actions** tab
3. You should see **"Deploy Zes Solutions to Hostinger"** workflow
4. If it hasn't run yet, make a small edit to any file and commit it

OR manually trigger:
- Click on the workflow name
- Click **Run workflow** → **Run workflow**

**Watch the deployment live** — green ✅ means success!

---

### STEP 6 — Point Your Domain to Hostinger

If you have a custom domain (e.g. `zessolutions.in`):

1. In hPanel → **Domains** → **DNS Zone Editor**
2. Make sure you have an **A record** pointing to your Hostinger server IP
3. Wait 15–60 minutes for DNS to propagate

Or if buying a new domain:
- Buy it directly from Hostinger → it auto-connects to your hosting

---

## 🔄 How Auto-Deploy Works

Every time you push a change to GitHub:

```
You edit index.html → Push to GitHub → GitHub Actions runs → Files upload to Hostinger → Website updates live ✅
```

**No manual FTP uploads ever again!**

---

## 🛠 Making Updates to the Website

1. Edit `index.html` on your computer (or directly on GitHub)
2. Commit and push to the `main` branch
3. GitHub Actions automatically deploys to Hostinger within ~2 minutes

---

## 📞 Support

- Email: hello@zessolutions.in  
- WhatsApp: +91 98XXX XXXXX

---

© 2025 Zes Solutions. Chennai, Tamil Nadu, India.
