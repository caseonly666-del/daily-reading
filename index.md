---
layout: default
title: 每日閱讀情報
---

# 每日閱讀情報

**每天一個值得理解的問題，5 分鐘看懂新聞背後真正重要的事。**

國際・財經・科技・地緣防務・東南亞・股市・書籍推薦

---

## 最新文章

{% for post in site.posts %}

### [{{ post.title }}]({{ site.baseurl }}{{ post.url }})

**{{ post.date | date: "%Y-%m-%d" }}｜{{ post.category }}**

{% if post.excerpt %}
{{ post.excerpt | strip_html | truncate: 120 }}
{% endif %}

---

{% endfor %}

## RSS 訂閱

使用 RSS 閱讀器的讀者，可訂閱：

[每日閱讀情報 RSS]({{ site.baseurl }}/feed.xml)
