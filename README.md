# Simplest Jekyll
> A Github Pages Jekyll site reduced to one page of content and a theme


## Live demo

- [michaelcurrin.github.io/simplest-jekyll/](https://michaelcurrin.github.io/simplest-jekyll/)


## How to use this project

### Setup

1. Click _Use this template_ to create a new repo in your own account. You can keep the name as `simplest-jekyll`.
2. Enable [GitHub Pages](https://pages.github.com/) in your repo's settings. Choose `master` branch and `/` path option.
3. Check your repo's _environment_ tab to see when the deploy is done.
4. Click _View deployment_ to see the live site.
    - See the the URL in the previous section.
    - Note that `/simplest-jekyll/index.html` is available immediately but it takes a few minutes until Github Pages makes `/simplest-jekyll/` available.

### Customize

- Update the `README.md` with your own details. This is not actually used in the deployed site but is visible locally and on Github.
- Themes
    - Edit the theme in [\_config.yml](/_config.yml) if you want another theme.
    - You can also use the Github Pages section of the repo Settings to preview visually. 
    - Note only themes supported by Github Pages are covered (about 10) but if you use the _remote_theme_ field in your config you can reference more themes.
    - For installing and running locally, you'll need to make sure your [Gemfile](/Gemfile) covers the theme used in the config.
- As with most Jekyll sites, the [index.md](/index.md) is used as the homepage. 
    - It has front matter at the top so any Liquid will be applied. 
    - Edit your `index.md` file with your own content as HTML or markdown. 
    - You can rename it to `index.html` if you only want plain HTML.
    - You can remove the front matter at the top to remove Liquid formatting and any theming.
- If you want to, add more pages at the root and break out any common HTMl such as header or head or navbar into `_includes` folder or `_layouts` folder (neither are covered in the scope of this project but are common for Jekyll projects).
- See the docs and tutorials on the [Jekyll](https:jekyllrb.com/) site for more info.
