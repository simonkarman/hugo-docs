# Hugo Documentation with GitHub Pages
This [repository](https://github.com/simonkarman/hugo-docs) shows how you can use [GitHub Pages](https://pages.github.com/) with [Hugo](https://gohugo.io/) to create a documentation hub for your repository. Created by [Simon Karman](https://www.simonkarman.nl).

You can find a demo of the publish docs here: [https://simonkarman.github.io/hugo-docs/](https://simonkarman.github.io/hugo-docs/).

## Getting started
After you have installed hugo on your machine. You can run hugo locally by using the following commands.
```bash
git submodule init
git submodule update
cd docs
hugo serve
```

The local web server should then be available at [localhost:1313](http://localhost:1313/). It has full reload capabilities enabled when you make changes locally, so you can easily test your changes locally. 

> Initialization of submodules is required to download the [Hugo theme](https://github.com/matcornic/hugo-theme-learn).

## Publish
The process of publishing the GitHub page is described in the `docs.yml` GitHub action in the `.github/workflows` folder. It uses `hugo --gc --minify --baseURL "<base-url-here>` to build the hugo website into static files.

Some things to keep in mind:
- The documentation is written in markdown and can be found within the `docs/content` folder.
- If you want to create links to other pages please follow [this](https://gohugo.io/content-management/cross-references/).
- Markdown pages should have a title and weight (so that the ordering is done consistently).

## Visibility
With a GitHub Enterprise account, you can restrict access to your GitHub Pages site by publishing it privately. A privately published site can only be accessed by people with read access to the repository the site is published from. You can use privately published sites to share your internal documentation or knowledge base with members of your enterprise.
