# LeanIX Report Gallery

![LeanIX Report Gallery icon](src/assets/images/lrg-icon-32x32.png)

The [LeanIX Report Gallery](https://stephen-gates.github.io/report-gallery/site/) helps Enterprise Architects who want to influence decisions by helping them quickly find and re-create reports that answer key questions.

- Discover the questions you can answer using LeanIX reports.
- Explore the different types of reports you can create.
- Share what you've made using the [LeanIX Enterprise Architecture Suite](https://www.leanix.net/en/solutions/enterprise-architecture-suite).

*This repository is in no way affiliated with [LeanIX](https://www.leanix.net/en/).* 

## About

- The site is built using [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- Pages are written in Markdown
- Site is configured using mkdoc.yml

## Dev

Run locally web server `$ mkdocs serve` to preview your site before publishing

Build `$ mkdocs build` creates html files in \site

Deploy `$ mkdocs gh-deploy` 

Go to https://stephen-gates.github.io/report-gallery/site/ to view the published site (there may be a small delay before the updates appear)

Keep things up-to-date:

`$ pip3 install --upgrade mkdocs-material`

or if using Insiders 

`pip3  install --upgrade  git+https://{GH_TOKEN}@github.com/squidfunk/mkdocs-material-insiders.git`
