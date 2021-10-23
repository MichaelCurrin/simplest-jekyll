# Simplest Jekyll
> A minimal Jekyll-based site on GH Pages, reduced to one page of content with a theme

[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/simplest-jekyll)](https://github.com/MichaelCurrin/simplest-jekyll/tags/?include_prereleases&sort=semver)
[![License](https://img.shields.io/badge/License-MIT-blue)](#license)

[![Ruby](https://img.shields.io/badge/Ruby->=2.6-blue?logo=ruby&logoColor=white)](https://ruby-lang.org)
[![Jekyll](https://img.shields.io/badge/Jekyll-3.9-blue?logo=jekyll&logoColor=white)](https://jekyllrb.com)


<div align="center">
    
[![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f?style=for-the-badge)](https://github.com/MichaelCurrin/simplest-jekyll/generate)

[![View site GH Pages](https://img.shields.io/badge/View_site-GH_Pages-blue?style=for-the-badge)](https://michaelcurrin.github.io/simplest-jekyll/)

</div>


## Preview

<div align="center">
    <a href="https://michaelcurrin.github.io/simplest-jekyll/">
        <img src="/sample.png" alt="Sample screenshot" title="Go to website" width="700" />
    </a>
</div>


## About

This is a template and live demo project. It shows how little you need to setup to get a Jekyll site on GH Pages.

- [index.md](/index.md)
    - For the homepage - the only page in this case.
    - If you leave out this page, then `README.md` will be used as your homepage.
- [\_config.yml](/_config.yml)
    - Set the theme - that handles the layout and styling.
    - Enable Jekyll Sitemap plugin - enabling it in Gemfile is not enough. Note that other plugins will be enabled for you like optional frontmatter.
    - Other standard values like `baseurl`, `title` and `description` have been left out of the config. When building on GH Pages, these will be inferred for you by the GH Pages gem.
- [Gemfile](/Gemfile)
    - This is not actually used by GH Pages, but it allows you to install the Jekyll theme locally using Bundler. 
    - Use a single gem `github-pages` if you want to match all the gems on GH Pages (which can be heavy to install). 
    - Delete this file if you don't need to run your site locally.

If you want a more full-fledged example of a multi-page site with posts, gems, layouts, etc. then checkout my [jekyll-blog-demo](https://github.com/MichaelCurrin/jekyll-blog-demo) repo. That can be used as a template and demo site too.


## How to use this project

### Setup

1. Click _Use This Template_ to create a new repo in your own account. You can leave the name as `simplest-jekyll`.
2. Enable [GitHub Pages](https://pages.github.com/) in your repo's settings. Choose to serve from `master` branch and the `/` path option.
3. Check your repo's _environment_ tab to see when the deploy is done.
4. Click _View deployment_ to see the live site. e.g. https://michaelcurrin.github.io/simplest-jekyll/

Note that `/simplest-jekyll/index.html` is available immediately but it takes a few minutes until Github Pages makes `/simplest-jekyll/` available.

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
- Optionally run Jekyll locally:
    - Install Ruby and [Bundler](https://bundler.io).
    - Install project gems - Jekyll and the theme gem.
    - Run Jekyll dev server.
    - For fuller instructions see [docs](https://github.com/MichaelCurrin/jekyll-blog-demo/tree/master/docs) of Jekyll Blog Demo. You'll need to add a `Makefile` as well to match those commands.


## Related projects


- [![MichaelCurrin - jekyll-blog-demo](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-blog-demo&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-blog-demo) - default blog generated with Jekyll CLI. Using a theme, content, style set up, gems, and a Makefile.
- [![MichaelCurrin - jekyll-gh-actions-quickstart](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-gh-actions-quickstart&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart) - using Jekyll 4, a theme, GitHub Actions, and GitHub Pages.
- [![MichaelCurrin - jekyll-themed-site-quickstart](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-blog-demo&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-blog-demo) - minimal Jekyll site with a theme but no Gemfile.


## License

Released under [MIT](/LICENSE) by [@MichaelCurrin](https://github.com/MichaelCurrin).
