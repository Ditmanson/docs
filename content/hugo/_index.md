---
title: "Hugo"
date: 2026-01-19T15:26:15Z
lastmod: 2026-01-19T15:26:15Z
publishdate: 2018-12-08T15:26:15Z
draft: false
weight: 1
description: Description not needed
images:
- images/pexels-photo-196666.jpeg
---
# My walkthrough
[Building a hugo site part 1](https://www.youtube.com/watch?v=Ri4XtitRAT0)

# Prerequisites 
- [install hugo cli](https://gohugo.io/installation/)
- [install git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [make github account](github.com)

## [Installation](./installation)
- [brew install hugo](https://brew.sh/) # mac
- sudo pacman -S hugo # arch
- sudo apt install hugo # debian
- sudo dnf install hugo # fedora
- [choco install hugo-extended](https://chocolatey.org/install) # windows

## From hugo's quickstart guide
```
hugo version
hugo new site quickstart
cd quickstart
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo "theme = 'ananke'" >> hugo.toml
hugo server
```

## How do we use hugo?
For the most part we do everything from the content folder. Make your markdown files as layed out in whatever theme you choose. Then we test with `hugo server` and check out how it looks at localhost:1313 from a browser. When we are ready to make our executables we run `hugo` then rsync the contents of the public directory to our pvc.

## [Configuration](./configuration)

You may specify options in hugo.toml (or hugo.yaml/hugo.json) of your site to make use of this theme's features.

I used to go through and change eveyrthing to yaml, but I find it's easier to just grab a templates example toml/json/yaml. If they don't have an example config file, I won't use that template. Not trying to read code with a tool like this.

Some templates require node. Anything that has `npm` in the instructions requires node to be installed. I pretty much just avoid those ones. npm package files are pretty heavy, probably the heaviest files in software development. If I need node, then I might as well use a real framework.

I'll leave more chapters for more detailed portions of using hugo. 

### Example of screen shot for this template.
![Image for later](../images/pexels-photo-196666.jpeg)
