# GetOutOfMyBakery Jekyll Blog
A scratchpad Jekyll blog for my personal GitHub account.

## Up and Running
1. Checkout this repo: `gh repo clone GetOutOfMyBakery/getoutofmybakery.github.io`
1. Update the variables in `.envrc`
1. Run: `bin/setup`
1. Run: `bin/dev`
1. The blog is now locally hosted at: [127.0.0.1:4000](http://127.0.0.1:4000/) _or_ [localhost:4000](http://localhost:4000/)

> [!TIP]
> Consider using a tool like [direnv](https://github.com/direnv/direnv) to automatically set the projects ENV vars.

> [!IMPORTANT]
> `bin/qr-code` displays a QR Code that can be used by a mobile device. The supplied IP address therefore needs to be something that can be routed, e.g.:
> - local address: `192.168.#.#`
> - hostname: `my-laptop.home.arpa`

## Creating and managing posts
With the help of [`jekyll-compose`](https://github.com/jekyll/jekyll-compose), creating and managing posts is easy:
``` shell
bundle exec jekyll post "My new post"
bundle exec jekyll draft "My new draft"

bundle exec jekyll help # Show the list of commands available to jekyll
```
See the `jekyll-compose` [Usage](https://github.com/jekyll/jekyll-compose?tab=readme-ov-file#usage) section for more.

## Updating the theme
Check out the `jekyll-theme-chirpy` [wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

You can also examine the latest version of the gem with:
```shell
bundle open jekyll-theme-chirpy
```
> [!IMPORTANT]
> In order to maintain the `Skip to main content` button, and some other minor tweaks, use `bin/diff-upstream-gem` to check for any relevant upstream changes that need to be merged in/resolved when updating versions.
> For ease of use remember that `bin/diff-upstream-gem` can pass in `chars` or `words` to the script to see just the different characters or words respectively.

Check how production will look before deploying with: `JEKYLL_ENV=production bin/dev`.

## Making a commit
[Lefthook](https://github.com/evilmartians/lefthook/) has been configured with pre-commit checks to:
- run `actionlint` for the `.github/workflows`
- run `htmlproofer` on the generated site
- run `shellcheck` on any shell or bash scripts

If for some reason it's necessary, it's possible to temporarily skip `lefthook` with: `LEFTHOOK=0 git commit`.

## Deploying changes
Simply merge to `main` and the [pages-deploy workflow](.github/workflows/pages-deploy.yml) will handle the building and deploying to [GitHub Pages](https://pages.github.com/).  
The site is currently hosted [here](https://getoutofmybakery.github.io/).
