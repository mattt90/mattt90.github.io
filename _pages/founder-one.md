---
title: "Founder One"
permalink: /founders/founder-one/
author: founder-one
author_profile: true
---

## Co-founder, Brew City Data

This is a generic founder profile, ready for a name, photo, and personal biography.
{: .notice--info}

Founder One's placeholder focus is the data foundation: how information is collected, organized, tested, and made useful.

### Areas of interest

- Data engineering and dependable pipelines
- Analytics and clear business definitions
- Data quality, documentation, and observability

### On the blog

{% assign founder_posts = site.posts | where: "author", page.author %}
{% for post in founder_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% else %}
Articles from this founder are coming soon.
{% endfor %}

[Meet the other co-founder]({{ '/founders/founder-two/' | relative_url }}) or [see the full team]({{ '/founders/' | relative_url }}).
