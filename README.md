# GetOutOfMyBakery GitHub Page (Jekyll)
A scratchpad Jekyll blog for my personal GitHub account.

## Up and Running
1. Checkout this repo: `gh repo clone GetOutOfMyBakery/getoutofmybakery.github.io`
1. Run: `bin/dev`
1. Navigate to: [127.0.0.1:4000](http://127.0.0.1:4000/) _or_ [localhost:4000](http://localhost:4000/)

## Deploying changes
Simply merge to `main`.

## Creating and managing posts
With the help of [`jekyll-compose`](https://github.com/jekyll/jekyll-compose), creating and managing posts is easy:
``` shell
bundle exec jekyll post "My new post"

bundle exec jekyll help # Show the list of commands available to jekyll
```
See the `jekyll-compose` [Usage](https://github.com/jekyll/jekyll-compose?tab=readme-ov-file#usage) section for more.

## Updating the theme
Check out the `jekyll-theme-chirpy` [wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

You can also examine the latest version of the gem with:
```shell
bundle open jekyll-theme-chirpy
```
