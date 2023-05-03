---
title: "Getting Started"
weight: 1
---

## Getting started
You can find the source code in the [GitHub repository (simonkarman/hugo-docs)](https://github.com/simonkarman/hugo-docs).

After you have installed hugo on your machine. You can run hugo locally by using the following commands.
```bash
git submodule init
git submodule update
cd docs
hugo serve
```

The local web server should then be available at [localhost:1313](http://localhost:1313/). It has full reload capabilities enabled when you make changes locally, so you can easily test your changes locally.

> Initialization of submodules is required to download the [Hugo theme](https://github.com/matcornic/hugo-theme-learn).
