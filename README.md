# Publish Privacy Policy Only (GitHub Pages)

Use these steps to publish only the privacy policy page, without exposing your game source code.

## 1) Create a separate public repository

Create a new repo on GitHub, for example:

- tilt9-privacy-policy

Do not create it from your game repo.

## 2) Upload only this folder's files

Upload these files to the new repo root:

- index.html
- README.md

Folder source in your local project:

- privacy-policy-site/

## 3) Enable GitHub Pages

In the new repo:

1. Go to Settings
2. Go to Pages
3. Under Build and deployment, choose:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /(root)
4. Save

GitHub will provide a URL like:

- https://YOUR_USERNAME.github.io/tilt9-privacy-policy/

## 4) Paste that URL into Play Console

Use this URL in the Privacy policy URL field.

## 5) Keep it updated

When policy text changes, update index.html in this pages repo and commit.

## Optional quick publish from terminal

If you want to push from terminal instead of web upload:

1. Open a terminal inside privacy-policy-site
2. Run:

   git init
   git add .
   git commit -m "Initial privacy policy site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/tilt9-privacy-policy.git
   git push -u origin main
