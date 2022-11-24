---
layout: post
title: Common Mistakes in using GitHub
author: YAP S S
date: '2018-10-09 13:11'
template: post
---

Some of the mistakes when I encounter using Git and GitHub for the first time

## Git push requires username and password

You cloned a git repository from your Github account to your PC. When you try to push to or pull from Github using your PC, it requires username and password every time.

### Using SSH

A common mistake is cloning using the default (HTTPS) instead of SSH. You can correct this by going to your repository, clicking "Clone or download", then clicking the "Use SSH" button above the URL field and updating the URL of your origin remote like this:

`git remote set-url origin git@github.com:USERNAME/REPOSITORY.git`

### Using HTTPS

If you're cloning GitHub repositories using HTTPS, you can use a credential helper to tell Git to remember your GitHub username and password every time it talks to GitHub.
```
`$ git config credential.helper store`
`$ git push https://github.com/repo.git`

Username for 'https://github.com': <USERNAME>`
Password for 'https://USERNAME@github.com': <PASSWORD>`
```