---
layout: default
title: Home
---

# Translated Articles

海外の記事・エッセイの日本語翻訳アーカイブです。

{% for article in site.articles %}
- [{{ article.title }}]({{ article.url | relative_url }})
  <br><small>{{ article.original_author }} | {{ article.date | date: "%Y-%m-%d" }} | [原文]({{ article.original_url }})</small>
{% endfor %}
