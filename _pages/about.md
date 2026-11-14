---
layout: about
title: about
permalink: /
subtitle:

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

这里放个人简介。改这个文件就是改首页内容。

想加头像就放一张 `assets/img/prof_pic.jpg`，然后在文件开头的 YAML 里加：

```yaml
profile:
  align: right
  image: prof_pic.jpg
  image_circular: false
```
