# GitHub Pages' Hugo page with a staging path 🧪

![GitHub last commit (branch)](https://img.shields.io/github/last-commit/timothechauvet/hugo-gh-pages-staging/main)

## What's this 🤓
GitHub Action that I developed for a GitHub Enterprise Server (GHES) instance because the usual actions wouldn't work. 

It does that :
1. clones & build the main branch and its Hugo page
2. clones & build the staging branch and its Hugo page
3. moves the staging Hugo page to the "/staging-env" path

## Usage 🤖
1. Take out that .yml file
2. Put it in your repo under `.github/workflows`
3. Configure it
4. Enjoy

## Configuration ⚙️
You must configure these in the .yml directly since I'm not uploading it as a template

- `push:` (line 5-8) : Remove if you prefer to build the staging environment manually
- `runs-on` (lines 21, 96) : If you're on a GHES server, usually you would go with "self-hosted"
- `HUGO_VERSION: 0.131.0` (line 27) : Hugo version to use
- `go-version: '1.22'` (line 40) : Go version to use
- `staging-env/` (lines 79, 85) : The path to which the staging environment URL must point to

## Contributions 🫵
For bugs, ideas or features requests, please submit an issue in this repository.

## Contact 🤗
- via LinkedIn : https://www.linkedin.com/in/timothechauvet/
- via Mail : timothe@chauvet.cloud
- or via an issue in this repository
