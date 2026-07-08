---
layout: home
title: AI Research Briefings
---

# 🤖 AI 研究简报

每日精选 arXiv AI 论文 + GitHub Trending 项目。

## 历史简报

| 日期 | 链接 |
|------|------|
{% for entry in site.data.briefings %}
| {{ entry.date }} | [查看简报]({{ entry.url | relative_url }}) |
{% endfor %}
{% for post in site.posts %}| {{ post.date | date: "%Y-%m-%d" }} | [查看简报]({{ post.url | relative_url }}) |
{% endfor %}
