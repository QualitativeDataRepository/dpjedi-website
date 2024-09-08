---
title: Data-PASS Journal Editors Discussion Interface
layout: jedi
toc: true
page_title: "Resources"
sidebar: true
join: true
post: false
---

{% capture resources_intro %}
{% include resources/resources-intro.md %}
{% endcapture %}
{{ resources_intro | markdownify }}

<!-- {% capture table_of_contents %}
{% include resources/table-of-contents.md %}
{% endcapture %}
{{ table_of_contents | markdownify }} -->

{% assign sections = "general,incoming-editors,ethics,diversifying-social-science-research,open-science,reconsideration-of-previously-rejected-submissions,improving-the-quality-of-reviews,peer-reviewing-tools-guidelines,incentivising-reviews,reviewer-editorial-collusion,detecting-overlap-between-submitted-existing-manuscripts,retraction,submission-types,peer-review-innovations,limitations-of-peer-review,editorial-secrets,formatting,persistence-preservation,list-of-contributors-to-this-page" | split: ',' %}

{% for section in sections %}
{% capture section_content %}
{% include resources/{{ section }}/{{ section }}.md %}
{% endcapture %}
{{ section_content | markdownify }}

{% assign sub_sections = site.data.resources.table-of-contents[section] %}
{% if sub_sections %}
{% for sub_section in sub_sections %}
{% capture sub_content %}
{% include resources/{{ section }}/{{ sub_section }}.md %}
{% endcapture %}
{{ sub_content | markdownify }}
{% endfor %}
{% endif %}
{% endfor %}