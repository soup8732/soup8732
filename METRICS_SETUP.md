# 🚀 Optional: Advanced GitHub Metrics Setup Guide

## ⚠️ Important Note

**Your README is fully functional without this setup!** This guide is for **optional advanced features** like:
- Snake contribution animation
- GitHub Achievements badges
- 3D Isometric calendar
- In-depth language analytics
- GitHub Skyline visualization
- Terminal-style portfolio

**You do NOT need to set this up** unless you want these extra visual features. Your current README already looks great and displays all standard GitHub stats.

## Step 1: Create a GitHub Personal Access Token

1. Go to **GitHub Settings** → **Developer settings** → **Personal access tokens** → **Tokens (classic)**
   - Or visit: https://github.com/settings/tokens
2. Click **Generate new token** → **Generate new token (classic)**
3. Give it a name like "GitHub Metrics"
4. Select the following permissions:
   - ✅ `public_repo` (or `repo` if you have private repos)
   - ✅ `read:user`
   - ✅ `repo:status`
5. Click **Generate token**
6. **COPY THE TOKEN** - you won't see it again!

## Step 2: Add Token as Repository Secret

1. Go to your repository: https://github.com/soup8732/soup8732
2. Click **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret**
4. Name: `METRICS_TOKEN`
5. Value: Paste your token from Step 1
6. Click **Add secret**

## Step 3: Enable GitHub Actions

1. Go to your repository: https://github.com/soup8732/soup8732
2. Click **Settings** → **Actions** → **General**
3. Under "Workflow permissions", select **Read and write permissions**
4. Click **Save**

## Step 4: Trigger the Workflows

After merging your PR to main:

1. Go to **Actions** tab in your repository
2. You'll see two workflows:
   - **Generate Snake Animation** - Creates the contribution snake
   - **Metrics** - Creates all the advanced metrics

3. Run both workflows:
   - Click on each workflow name
   - Click **Run workflow** → **Run workflow**
   - Wait 2-3 minutes for generation to complete

The snake animation will appear first (fastest), then the metrics will populate.

## Step 5: Verify

Once the workflows complete:
- Check your repository for new `.svg` files (metrics.plugin.*.svg)
- Your README will automatically display the beautiful metrics!

## Automatic Updates

Both the snake animation and metrics will automatically update:
- ⏰ Daily (snake every 24 hours, metrics at midnight UTC)
- 🔄 Every time you push to main/master branch
- 🎯 Manually via Actions tab anytime

**Note:** The snake animation uses the default GitHub token (no setup needed). The advanced metrics require the METRICS_TOKEN.

## Troubleshooting

**Metrics not showing?**
- Make sure METRICS_TOKEN secret is set correctly
- Check the Actions tab for any errors
- Ensure the workflow has completed successfully
- Clear your browser cache or view in incognito mode

**Need help?**
- Check the workflow logs in the Actions tab
- Visit: https://github.com/lowlighter/metrics

---

Enjoy your stunning GitHub profile! 🎉
