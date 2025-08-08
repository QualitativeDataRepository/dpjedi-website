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
<h2> Events organized by the JEDI Team </h2>
<br>

{% capture events-intro %}
{% include /events/events-intro.md%}
{% endcapture %}
{{ events-intro | markdownify }}

<br>

<header class="major">
  <h2>Data-PASS Events</h2>
  <p><b>The following workshops with journal editors were organized by the same group of repositories that went on to launch JEDI (Data-PASS), and were important catalysts of its creation.</b></p>
</header>
<br>

{% capture events-data-pass-events %}
{% include /events/events-data-pass-events.md%}
{% endcapture %}
{{ events-data-pass-events | markdownify }}


</section>
</div>
</div>