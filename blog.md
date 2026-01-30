---
layout: home
title: Fulcria Labs Blog
permalink: /blog/
---

# Golf Tech Insights

Welcome to the Fulcria Labs blog. We share tips on improving your golf swing, insights from AI-powered analysis, and practical advice for golfers of all skill levels.

<div style="background: linear-gradient(135deg, #1a472a 0%, #2d5a3d 100%); padding: 24px; border-radius: 12px; margin: 24px 0; text-align: center;">
  <h3 style="color: #fff; margin: 0 0 12px 0; font-size: 1.3em;">Ready to see your swing differently?</h3>
  <p style="color: #c8e6c9; margin: 0 0 16px 0;">Get instant AI feedback in 90 seconds. No tripod. No waiting.</p>
  <a href="https://swing.fulcria.com" style="display: inline-block; background: #4CAF50; color: white; padding: 14px 32px; border-radius: 8px; text-decoration: none; font-weight: bold; font-size: 1.1em;">Try Swing Analyzer Free</a>
</div>

---

## Latest Posts

{% for post in site.posts limit:10 %}
### [{{ post.title }}]({{ post.url | relative_url }})
{{ post.excerpt | strip_html | truncatewords: 50 }}

*{{ post.date | date: "%B %d, %Y" }}* | {{ post.categories | join: ", " }}

---
{% endfor %}
