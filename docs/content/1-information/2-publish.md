---
title: "Publish"
weight: 2
---

Please follow the guide in [Getting Started]({{< relref "./1-getting-started" >}}) first. You can find the source code in the [GitHub repository (simonkarman/hugo-docs)](https://github.com/simonkarman/hugo-docs).

## Publish
The process of publishing the GitHub page is described in the `docs.yml` GitHub action in the `.github/workflows` folder. It uses `hugo --gc --minify --baseURL "<base-url-here>` to build the hugo website into static files.

This means that all you have to do is push a new commit to the main branch and the GitHub page will be created or update according to your changes.

> Note: make sure to update the `docs/config/production/config.toml` file with the base url of your GitHub page. 

You can find the running example here: [https://simonkarman.github.io/hugo-docs/](https://simonkarman.github.io/hugo-docs/) based on [GitHub repository (simonkarman/hugo-docs)](https://github.com/simonkarman/hugo-docs).

### Visibility
By default, your page will be visible to the internet. Be wise about what you share.

With a GitHub Enterprise account, you can restrict access to your GitHub Pages site by publishing it privately. A privately published site can only be accessed by people with read access to the repository the site is published from. You can use privately published sites to share your internal documentation or knowledge base with members of your enterprise.
