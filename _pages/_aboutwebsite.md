---
title: "About the website"
layout: textlay
excerpt: "About the website."
sitemap: false
permalink: /aboutwebsite.html
---

### Getting started
All pages are written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for easy editing, and [Jekyll](https://jekyllrb.com) uses Liquid for the data-driven pages. 

The publicaion list, news items, and group members are stored as `.yml` data sheets (plain text) in the `_data folder`, so that one can update the website easily. 

The pages are in the `_pages` folder. 

`_data` folder
- `news.ylm`
    - important  news items (red, "news1"), and less important  news items (blue, "news2").
    - For the news items, just keep adding them. The first 10 will be displayed on the 'home' page.
- `publist.ylm`
    - add a "1" in the highlight field to feature
- `team.ylm` 

To change the title in the homepage, go to `homelay.html` in the `_layout` folder.
Lastly, change the footer and perhaps header appropriately (in `_include`).

