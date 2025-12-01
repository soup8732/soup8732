# 🚀 GitHub Metrics Setup Guide

Your README now includes advanced GitHub metrics! Follow these steps to activate them:

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

## Step 3: Trigger the Workflow

After pushing your changes:

1. Go to **Actions** tab in your repository
2. Click on **Metrics** workflow
3. Click **Run workflow** → **Run workflow**
4. Wait 2-3 minutes for all metrics to generate

## Step 4: Verify

Once the workflow completes:
- Check your repository for new `.svg` files (metrics.plugin.*.svg)
- Your README will automatically display the beautiful metrics!

## Automatic Updates

The metrics will automatically update:
- ⏰ Daily at midnight UTC
- 🔄 Every time you push to main/master branch
- 🎯 Manually via Actions tab

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
