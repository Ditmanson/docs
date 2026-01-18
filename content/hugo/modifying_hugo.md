---
title: "Modifying Hugo Content"
date: 2026-01-16T15:26:15Z
lastmod: 2026-01-16T15:26:15Z
publishdate: 2026-01-16T15:26:15Z
draft: false
weight: 2
description: Description not needed
---

# Hugo Content
All your markdown files in the content and content/child directories are what's used to render the html later. This is why I like an example site. Different themes set up static files and folders differently. They usually have good instructions; however, I think it's easiest just to grab an example site and edit everything in the content folder, one file at a time and then check it with `hugo server`. 

Each theme also has a header key value pair header that is used in rendering the content. Here's what this page looks like:
```
---
title: "Modifying Hugo Content"
date: 2026-01-16T15:26:15Z
lastmod: 2026-01-16T15:26:15Z
publishdate: 2026-01-16T15:26:15Z
draft: false
weight: 2
description: Description not needed
---
```
The weight tells this site where to place the order of the folders. Lower numbers go higher, higher numbers go lower. Some themes order their lists with the date. On this particular theme the description seems pretty useless. It can be annoying to remember how each header is supposed to be engineered, so to avoid mistakes I create new markdown files from the terminal with the head command. For this one I used `head -8 picking_a_template.md > modifying_hugo.md`. 

Then when I opened the file I just edited the title. 

For the date, if your a vim user from inside vim run: `:r !date -u '+%Y-%m-%dT%H:%M:%SZ'`. 

