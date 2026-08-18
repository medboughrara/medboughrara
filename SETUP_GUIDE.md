# Complete GitHub Profile README Setup Guide for `@medboughrara`

This step-by-step guide walks you through publishing your personalized profile page to GitHub and initializing the automated WakaTime stats workflow.

---

## 📌 Phase 1: Create the Secret Repository on GitHub

GitHub displays the `README.md` of a repository on your profile page if the repository name **matches your exact GitHub username**.

1. Go to [github.com/new](https://github.com/new).
2. Set **Repository name** to: `medboughrara` *(a special green notification with a cat icon will confirm you've found the secret repository!)*.
3. Description *(optional)*: `Mouhamed Boughrara - Personal Profile & Automation README`
4. Set visibility to **Public** *(required for profile READMEs)*.
5. Do **NOT** initialize with a README, .gitignore, or license *(since we already created all files locally)*.
6. Click **Create repository**.

---

## 🔑 Phase 2: Add WakaTime API Key to GitHub Secrets

The GitHub Action automatically updates your profile stats using your WakaTime Secret API Key.

1. Open your newly created repository on GitHub: `https://github.com/medboughrara/medboughrara`
2. Navigate to **Settings** > **Secrets and variables** > **Actions**.
3. Click the green button **New repository secret**.
4. **Name**: `WAKATIME_API_KEY`
5. **Secret**: `<YOUR_WAKATIME_API_KEY>` (e.g. from your WakaTime Account Settings)
6. Click **Add secret**.

---

## 🚀 Phase 3: Push Local Files to GitHub

Run the following shell commands from the `medboughrara` folder:

```bash
# Navigate to the folder containing your profile files
cd d:/smart_scan/SmartCytoScan/medboughrara

# Initialize git repository
git init

# Stage all files including .github/workflows/waka.yml and README.md
git add .

# Create initial commit
git commit -m "feat: setup personalized profile README with WakaTime automation"

# Set default branch to main
git branch -M main

# Link remote GitHub repository
git remote add origin https://github.com/medboughrara/medboughrara.git

# Push to GitHub
git push -u origin main
```

---

## ⚡ Phase 4: Trigger the WakaTime Action Immediately

Once pushed:
1. Go to your repository **Actions** tab: `https://github.com/medboughrara/medboughrara/actions`
2. On the left sidebar, click on **WakaTime Status Update**.
3. Click on the **Run workflow** dropdown on the right side.
4. Click the green **Run workflow** button.
5. Wait ~30 seconds for the green checkmark ✔️.
6. Visit your GitHub profile page at **[github.com/medboughrara](https://github.com/medboughrara)** to view your dynamic profile!

---

## ⚙️ WakaTime IDE Extension Setup (If not already installed)

To track your coding activity in your editor (VS Code, CLion, PyCharm, etc.):
1. Open VS Code Extensions (`Ctrl+Shift+X`).
2. Search for `WakaTime` and click **Install**.
3. When prompted in VS Code, paste your Secret API Key (from WakaTime Settings > Account).
4. Code as normal—WakaTime will automatically track your stats and update your GitHub profile every night!
