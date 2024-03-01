---
layout: post
title: Inaugural Post
date: 2024-03-01 02:03 +0000
description: Initial post with Jekyll
tags:
- first-post
- tips
- markdown
- jekyll
- cheatsheet
published: true
pin: false
---
This is the first post to demonstrate that things are working correctly.

<!-- Create an alias: {:xn} to use as a suffix on links to create external link -->
{:xn: target="_blank" rel="nofollow noreferrer noopener"}

## Links
Here are some useful links:
- the [README](https://github.com/GetOutOfMyBakery/getoutofmybakery.github.io/blob/main/README.md){:target="_blank"}{:rel="noopener noreferrer"} for this blog
- the [Jekyll docs](https://jekyllrb.com/){:xn}
- the [Chripy theme's wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki){:xn}
- a [Chripy cheatsheet](https://chirpy.cotes.page/posts/text-and-typography/){:xn} with some help on supported features
- the [kramdown docs](https://kramdown.gettalong.org/syntax.html){:xn}

## Tips
```md
# Creating a link that opens externally:
[text](link){:target="_blank"}

# Creating a link that opens externally with noopener noreferrer:
[text](link){:target="_blank"}{:rel="noopener noreferrer"}

# To reduce copy+pasting this, you can create an alias with:
{:xn: target="_blank" rel="nofollow noreferrer noopener"}

# Then simply use:
[text](link){:xn}
```
