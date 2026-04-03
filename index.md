---
layout: home
title: AI Research Briefings
---

# 🤖 AI 研究简报

每日精选 arXiv AI 论文 + GitHub Trending 项目。

## 历史简报

| 日期 | 链接 |
|------|------|
{% for post in site.posts limit:30 %}| {{ post.date | date: "%Y-%m-%d" }} | [查看简报]({{ site.baseurl }}{{ post.url }}.html) |
{% endfor %}
