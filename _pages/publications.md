---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

This page shows my research publications.

{% include base_path %}

{% assign show_preprints = false %}
{% if show_preprints %}
Preprints
------
{% endif %}
{% for post in site.publications reversed %}
  {% if post.include_on_website %}
    {% include publication-single.html %}
  {% endif %}
{% endfor %}
