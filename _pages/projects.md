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
