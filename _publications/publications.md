---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

{% assign publications = site.publications | sort: 'date' | reverse %}
{% for post in publications %}
  <div class="publication-item">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p><strong>{{ post.venue }}</strong>, {{ post.date | date: "%Y" }}</p>
    <p>{{ post.excerpt }}</p>
    {% if post.paperurl %}
      <p><a href="{{ post.paperurl }}">View Paper</a></p>
    {% endif %}
    <hr>
  </div>
{% endfor %}

<p>You can also find my articles on my
<a href="https://scholar.google.com/citations?user=X3VSk2oAAAAJ&hl=en">Google Scholar profile</a>.</p>
