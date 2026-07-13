---
layout: home
title: AI Research Briefings
---

# 🤖 AI 研究简报

每日精选 arXiv AI 论文 + GitHub Trending 项目。

## 历史简报

<table>
  <thead>
    <tr>
      <th>日期</th>
      <th>链接</th>
    </tr>
  </thead>
  <tbody>
    {% for entry in site.data.briefings %}
    <tr>
      <td>{{ entry.date }}</td>
      <td><a href="{{ entry.url | relative_url }}">查看简报</a></td>
    </tr>
    {% endfor %}
    {% for post in site.posts %}
    <tr>
      <td>{{ post.date | date: "%Y-%m-%d" }}</td>
      <td><a href="{{ post.url | relative_url }}">查看简报</a></td>
    </tr>
    {% endfor %}
  </tbody>
</table>
