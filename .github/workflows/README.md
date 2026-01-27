# GitHub Actions Workflow

This workflow automatically builds and deploys the Hugo site to GitHub Pages.

## Setup Instructions

1. **Create a Personal Access Token (PAT)**:
   - Go to GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
   - Click "Generate new token (classic)"
   - Give it a descriptive name like "Hugo Deploy Token"
   - Select scopes:
     - `repo` (Full control of private repositories)
   - Click "Generate token"
   - Copy the token (you won't see it again!)

2. **Add the token as a repository secret**:
   - Go to your source repository: https://github.com/neoKushan/neoKushan.github.io.source
   - Navigate to Settings → Secrets and variables → Actions
   - Click "New repository secret"
   - Name: `PAGES_DEPLOY_TOKEN`
   - Value: Paste your PAT
   - Click "Add secret"

3. **The workflow will now**:
   - Trigger on every push to the `master` branch
   - Install Hugo 0.154.5 (extended)
   - Install Node.js 22 and pnpm 10.14.0
   - Install dependencies with `pnpm install`
   - Build the site with `pnpm run build` (Hugo + Pagefind)
   - Deploy the `public/` directory to `neoKushan/neoKushan.github.io` repository

## Manual Trigger

You can also manually trigger the workflow:
- Go to Actions tab in your repository
- Select "Deploy to GitHub Pages" workflow
- Click "Run workflow"

## Build Status

The workflow status will show in the Actions tab and on your repository README if you add a badge:

```markdown
![Deploy Status](https://github.com/neoKushan/neoKushan.github.io.source/workflows/Deploy%20to%20GitHub%20Pages/badge.svg)
```
