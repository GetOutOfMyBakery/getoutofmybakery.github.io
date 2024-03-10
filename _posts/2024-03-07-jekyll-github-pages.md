---
layout: post
title: Jekyll & GitHub Pages
date: 2024-03-07 22:22 +0000
description: 'A brief overview of my initial experience setting up Jekyll with GitHub Pages'
image:
  path: https://jekyllrb.com/img/octojekyll.png
  alt: GitHub's Mascot, Octocat, holding the Jekyll logo (a vial with red liquid) in one of it's tentacles. The image is from the Jekyllrb.com landing page.
# categories:
# - 
tags:
- tech
- development
- automation
- jekyll
- github
published: true
pin: false
---
{:xn: target="_blank" rel="nofollow noreferrer noopener"}

## Setting up my first Jekyll blog and deploying to GitHub Pages
My first impression of [Jekyll][jekyll-docs]{:xn} is extremely positive.

The _TL;DR_ version is that it's a Ruby-based static site generator, ideally suited for blogs, and optimized for GitHub Pages deployment, meaning you can have a blog online in just a few minutes that deploys in around 20 seconds.

Overall:
- it's super straightforward to [set up][jekyll-docs]
- the experience of [trying out an existing theme][jekyll-docs-themes]{:xn} and tweaking it for my own preferences was simple, intuitive, and demonstrates just how flexible an option Jekyll is
- configuring [GitHub Pages][github-pages] for deployment was again [well documented][chirpy-deploy-docs] and easy to [customize for my own needs and preferred workflow][my-deploy-pages-workflow]{:xn}

## Digging into some of the specifics
Once the [initial setup][inaugural-post] was in place, I took some time to:
- prioritize first time set up (i.e. up-and-running) and on-going development experience: 
  - [README.md][my-blog-readme]{:xn}
  - [`bin/setup` & `bin/dev`][my-bin-dir]{:xn} - simple entry points and quality of life configuration (auto-install, hot reloading, etc.)
- configure [lefthook][lefthook]{:xn} (a Go-based Git hooks manager) to ensure consistency going forwards:
  - [lefthook config][lefthook-config]{:xn}: static analysis tooling on a pre-commit hook
- configure [dependabot][dependabot-config]{:xn} for dependency management
- configure [editorconfig][editorconfig]{:xn}
- generally smoothed the development and deployment process (only relevant changes are deployed on merging back to the default branch, deployment takes around 20 seconds)
- set up [goatcounter][goatcounter]{:xn} for simple web analytics without tracking

All of this was pretty painless and only took a few hours over two evenings, that includes my first two posts [1][inaugural-post]{:xn},[2][zentangle-organised-chaos]{:xn}, as well the fact I was slightly pre-occupied rewatching [_Poor Things_ (2023)][poor-things]{:xn}. All in all an effortless setup.

***

[jekyll-docs]: https://jekyllrb.com/
[jekyll-docs-themes]: https://jekyllrb.com/docs/themes/
[github-pages]: https://pages.github.com/
[chirpy-deploy-docs]: https://chirpy.cotes.page/posts/getting-started/
[my-deploy-pages-workflow]: https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/blob/main/.github/workflows/pages-deploy.yml
[inaugural-post]: /posts/inaugural-post/
[my-blog-readme]: https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/blob/main/README.md
[lefthook]: https://github.com/evilmartians/lefthook/
[my-bin-dir]: https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/tree/main/bin
[lefthook-config]: https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/blob/main/lefthook.yml
[dependabot-config]: https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/blob/main/.github/dependabot.yml
[editorconfig]: https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/blob/main/.editorconfig
[goatcounter]: https://www.goatcounter.com/
[poor-things]: https://www.imdb.com/title/tt14230458/
[zentangle-organised-chaos]: /posts/zentangle-organised-chaos/
