---
title: Data-PASS Journal Editors Discussion Interface
layout: jedi
page_title: "Resources"
sidebar: true
join: true
post: false
---

{% capture resources_intro %}
{% include resources/resources-intro.md %}
{% endcapture %}
{{ resources_intro | markdownify }}

{% assign sections = site.data.resources.table-of-contents %}

{% for section in sections %}
{% assign section_file = section[0] %}
{% capture section_content %}
{% include resources/{{ section_file }}.md %}
{% endcapture %}
{{ section_content | markdownify }}
{% endfor %}