# Afkanerd Blog Website

This site is built using [Hugo](https://gohugo.io/) - a static site generator.

This repository is for writing content and most of the site's configurations. Changes to the design should be made in [this repo's theme](https://github.com/Afkanerd/hugo-theme-fuji) which happens to be a submodule in this repo.

## Building the site locally
- Follow these [steps](https://gohugo.io/getting-started/installing/) to install Hugo. Make sure to install the extended version.
- Clone the repo
```bash
git clone --recurse-submodules git@github.com:Afkanerd/afkanerd.github.io.git
```
- Run `hugo serve` to build the static site and open the localhost link on your terminal.

## Adding content to the site
- Create a markdown file in the `content/post` directory.
- The first part of your file **must** consist the [front matter](https://gohugo.io/content-management/front-matter/) which can be in `toml` or `yaml` or `json` format. Use the `toml` format here for consistency. It contains basic information about your post.
- Your front matter should look like this
```toml
+++
title = "Your post title"
date = "YYYY-MM-DD"
description = "A short description"
tags = ["tag1", "tag2", "tag3", etc]
+++
```
- Tags could be any keyword(s) about your content that can be used to filter the content. If you're not yet ready to publish the content, you can add `draft = true` to the front matter. Once you're ready to publish, change it to `false` and commit.
- Once you have the front matter, write your content underneath in markdown syntax.
- You can checkout the format of the sample markown file at `content/post/markdown-example.md`
- You can now commit and push your changes
