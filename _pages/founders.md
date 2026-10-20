---
title: "Meet the Founders"
permalink: /founders/
---

Two founders, complementary perspectives, and a shared interest in making data and AI work better.

These are placeholder profiles. Names and biographies will be updated as Brew City Data's team details are published.
{: .notice--info}

<div class="bcd-grid">
  {% for founder in site.data.authors %}
    {% assign profile = founder[1] %}
    <article class="bcd-card">
      <span class="bcd-eyebrow">Co-founder</span>
      <h2><a href="{{ profile.home | relative_url }}">{{ profile.name }}</a></h2>
      <p>{{ profile.bio }}</p>
      <a href="{{ profile.home | relative_url }}">Read the profile &rarr;</a>
    </article>
  {% endfor %}
</div>
