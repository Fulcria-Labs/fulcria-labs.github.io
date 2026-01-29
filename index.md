---
layout: home
title: Fulcria Labs Blog
---

# Golf Tech Insights

Welcome to the Fulcria Labs blog. We share tips on improving your golf swing, insights from AI-powered analysis, and practical advice for golfers of all skill levels.

**[Try Swing Analyzer](https://swing.fulcria.com)** - Get instant AI feedback on your swing in 90 seconds.

---

## Latest Posts

{% for post in site.posts limit:10 %}
### [{{ post.title }}]({{ post.url | relative_url }})
{{ post.excerpt | strip_html | truncatewords: 50 }}

*{{ post.date | date: "%B %d, %Y" }}* | {{ post.categories | join: ", " }}

---
{% endfor %}
