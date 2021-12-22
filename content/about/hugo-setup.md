---
title: Hugo Setup
description : "Doc of this site's setup"
---

# Hugo Setup for WT1
#wt1/
#hugo

## Setting up the site
- Strategy: copy the example site of the theme adapt it from there.
- used [Quick Start | Hugo](https://gohugo.io/getting-started/quick-start/) as a reference
	- Step 1 - install hugo (already done)
	- Step 2 - Create a new Site
		- copied theme example site:
 `cp -r hugo-theme-learn/exampleSite webbook`
	- Step 3 - add a theme
		- forked theme and cloned it (in case we want to adapt something) `git clone git@github.com:htw-imi-wt1-ws2021/hugo-theme-learn.git`
		- add theme
```
cd webbook
git init
git add .
git commit -m "copy exampleSite"
git submodule add git@github.com:htw-imi-wt1-ws2021/hugo-theme-learn.git themes/hugo-theme-learn-wt1
git status
less .gitmodules
git commit -m "add theme as submodule"
```
- add theme to config (edit config, see commit)
- here I left the path of the Quick start and also stopped recording all commands.
	- Step 5: start the server `hugo server`

## Deployment to github pages
- [Quickstart for GitHub Pages - GitHub Docs](https://docs.github.com/en/pages/quickstart)
- - the quickstart only describes the possibility of a gh generated page (using jekyll)
- create repo with repository name:
- `git@github.com:htw-imi-wt1-ws2021/htw-imi-wt1-ws2021.github.io.git`
- add github action  (see repo) using this action:
-  [peaceiris/actions-gh-pages: GitHub Actions for GitHub Pages 🚀 Deploy static files and publish your site easily. Static-Site-Generators-friendly.](https://github.com/peaceiris/actions-gh-pages)
- in Repo -> Settings -> Pages select gh_pages branch for publishing (this is the default used by the action) (gh_pages branch needs to be there already)
