---
title: Data-PASS Journal Editors Discussion Interface
layout: jedi
page_title: "JEDI Events"
permalink: /events/
redirect_from:
  - /events.html
---

<style>
  hr {
    border: 0;
    height: 1px;
    width: 50%;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
  }  
</style>

<div id="main" class="wrapper style1">
<div class="container">
<section>


{% capture events-intro %}
{% include /events/events-intro.md%}
{% endcapture %}
{{ events-intro | markdownify }}

<header class="major">
  <h1>Data-PASS Events</h1>
  <h4>The workshops with journal editors below were organized by the same group of repositories that went on to launch JEDI and were important catalysts for that platform.</h4>
</header>
<br>

{% capture events-data-pass-events %}
{% include /events/events-data-pass-events.md%}
{% endcapture %}
{{ events-data-pass-events | markdownify }}


</section>
</div>
</div>