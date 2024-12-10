---
title: Data-PASS Journal Editors Discussion Interface
layout: jedi
page_title: "Resources"
sidebar: true
join: true
post: false
permalink: /resources/
redirect_from:
  - /resources.html
---

{% assign sections = site.data.resources.table-of-contents %}

<div id="contentWrapper">
{% for section in sections %}
{% assign section_file = section[0] %}
{% capture section_content %}
{% include resources/{{ section_file }}.md %}
{% endcapture %}
<div id="{{ section_file }}">
{{ section_content | markdownify }}
</div>
{% endfor %}
</div>