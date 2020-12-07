---
layout: archive
title: "Project Posts by Tags"
permalink: /projects/
author_profile: true
header:
    image: "/assets/images/header.jpg"
---

{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
    {% assign posts = group_items[forloop.index0] %}
    <h2 class="archive__subtitle"> {{ tag }} </h2>

    {% for post in posts %}
        {% include archive-single.html %}
    {% endfor %}
{% endfor %}
