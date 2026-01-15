# playa

This repository was created to host the static site currently available at https://playa.vercel.app.

This repo is initially a skeleton created by GitHub Copilot. To publish the actual static site, either:

1) Upload a ZIP file of the built/static site here (attach it in this chat) and I will extract and push the files into the `gh-pages` branch for GitHub Pages.

2) Or run these commands locally to mirror the live site and push it to GitHub Pages yourself:

```bash
# mirror the public site locally
wget --mirror --convert-links --adjust-extension --page-requisites --no-parent https://playa.vercel.app/

# create repo clone (replace with your fork/clone URL)
git clone https://github.com/isaacsstiven10/playa.git
cd playa

# copy mirrored files into repo (example assumes wget output in ./playa.vercel.app)
cp -r ../playa.vercel.app/* .

# commit to gh-pages branch
git checkout -b gh-pages
git add .
git commit -m "Publish static site from playa.vercel.app"
git push -u origin gh-pages
```

Notes:
- If you prefer the built files in the `main` branch instead of `gh-pages`, tell me and I can adjust.
- License: MIT (included). Change if you prefer a different license.
