---
chapter: true
---

# Hugo Docs Example

Welcome to an example documentation setup using GitHub pages and hugo.

This repository shows how you can use GitHub Pages with Hugo to create a documentation hub for your repository. Created by [Simon Karman](https://www.simonkarman.nl).

### Getting started
To run hugo locally you can run the following commands.

```bash
git submodule init
git submodule update
hugo serve
```

### Publish
The process of publishing the GitHub page is described in the `docs.yml` GitHub action in the `.github/workflows` folder.

It uses `hugo --gc --minify --baseURL "{{.DOCS_BASE_URL}}/` to build the hugo website into static files.

### Chapters
Take a look at some chapters here

 [Example Chapter](1-example-chapter/) • [Example Chapter](2-example-chapter/) • [Simon Karman](https://www.simonkarman.nl)
