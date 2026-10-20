---
title: "Founder Two"
permalink: /founders/founder-two/
author: founder-two
author_profile: true
---

## Co-founder, Brew City Data

This is a generic founder profile, ready for a name, photo, and personal biography.
{: .notice--info}

Founder Two's placeholder focus is applied AI: exploring where models help, how to evaluate them, and when a simpler approach is the better choice.

### Areas of interest

- Applied AI and useful automation
- Evaluation, experimentation, and human feedback
- Responsible product design and privacy

### On the blog

{% assign founder_posts = site.posts | where: "author", page.author %}
{% for post in founder_posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% else %}
Articles from this founder are coming soon.
{% endfor %}

[Meet the other co-founder]({{ '/founders/founder-one/' | relative_url }}) or [see the full team]({{ '/founders/' | relative_url }}).
