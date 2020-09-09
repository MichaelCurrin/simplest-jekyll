# Simplest Jekyll
> A minimal Jekyll-based site on GH Pages, reduced to one page of content with a theme

[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/simplest-jekyll)](https://github.com/MichaelCurrin/simplest-jekyll/tags/?include_prereleases&sort=semver)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue)](#license)

<div align="center">
    
[![View site GH Pages](https://img.shields.io/badge/View_site-GH_Pages-green?style=for-the-badge)](https://michaelcurrin.github.io/simplest-jekyll/)
[![Use this template](https://img.shields.io/badge/Use_this_template-2ea44f?style=for-the-badge)](https://github.com/MichaelCurrin/simplest-jekyll/generate)

</div>

## Preview

<div align="center">
    <a href="https://michaelcurrin.github.io/simplest-jekyll/">
        <img src="/sample.png" alt="Sample screenshot" title="Sample screenshot" width="auto" height="300" />
    </a>
</div>


## About

This is a template and live demo project. It shows how little you need to setup to get a Jekyll site on GH Pages.

- `index.md` 
    - For the homepage, the only page in this case.
    - If you leave out this page, then `README.md` will be used as your homepage.
- `_config.yml` 
    - for the theme. That handles the layout and styling.
    - Other standard values like baseurl, title and description have been left out. When building on GH Pages, these will be inferred for you by the GH Pages gem.
- `Gemfile` 
    - Not actually used by GH Pages but it allows you to install the theme locally.

If you want a more full-fledged example of a multi-page site with posts, gems, layouts, etc. then checkout my [jekyll-blog-demo](https://github.com/MichaelCurrin/jekyll-blog-demo) repo. That can be used as a template and demo site too.


## How to use this project

### Setup

1. Click _Use This Template_ to create a new repo in your own account. You can leave the name as `simplest-jekyll`.
2. Enable [GitHub Pages](https://pages.github.com/) in your repo's settings. Choose to serve from `master` branch and the `/` path option.
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
- Running Jekyll locally
    - You might choose to add `gem 'jekyll', '~> 3.9` to the `Gemfile` and install it as a project gem.
    - Or just use a globally-installed Jekyll for your user.
    - [Bundler](https://bundler.io) is recommended for installing gems and running Jekyll.
    

## License

Released under [MIT](/LICENSE).
