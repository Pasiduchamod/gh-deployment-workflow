# GitHub Pages Deployment

This repo shows how to automatically deploy a static website to **GitHub Pages** using **GitHub Actions**.

## How it Works

- The workflow is in `.github/workflows/deploy.yml`.
- It runs when `index.html` is updated on the `main` branch.
- Steps:
  1. Checkout the code
  2. Prepare GitHub Pages
  3. Upload files
  4. Deploy the site

## Usage

1. Make sure you have `index.html` in your repo root.
2. Push changes to the `main` branch.
3. Your site will be live at:

https://"your-username".github.io/"repository-name"/


## Tips

- Make sure the workflow has correct permissions: `pages: write`, `contents: read`, `id-token: write`.
- You can trigger deployment for other files by updating the `paths` in the workflow.

  
## Project Idea Source
URL : https://roadmap.sh/projects/github-actions-deployment-workflow
