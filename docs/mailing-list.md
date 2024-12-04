---
title: JEDI Mailing List
layout: jedi
page_title: "JEDI Mailing List"
sidebar: false
join: true
post: true
---

<!-- <head>
    <style>
    .column {
    float: left;
    }
    .left-col {
    width: 60%;
    }
    .right-col {
    width: 40%;
    padding-bottom: 0%;
    }
    /* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
    @media screen and (max-width: 600px) {
    .column {
        width: 100%;
    }
    } 
    /* Clear floats after the columns */
    .row:after {
    content: "";
    display: table;
    clear: both;
    }
    </style>
</head> -->

<div class="container-fluid g-0">
    <div class="row">
        <div class="col-md-8">
{% capture markdown_part1 %}
{% include /mailing-list/mailing-list-intro.md%}
{% endcapture %}
{{ markdown_part1 | markdownify }}
        </div>
        <div class="col-md-4">
            <iframe name="JEDI Intro Video" width="100%" height="330" src="https://www.youtube.com/embed/d5vlNFBMBT8?si=1AbTtxpYAOsvkYWS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        </div>
    </div>
    <div class="row">
        <div class="col-md-12">
{% capture mailing-list-markdown %}
{% include /mailing-list/mailing-list-cont.md%}
{% endcapture %}
{{ mailing-list-markdown | markdownify }}
        </div>
    </div>
</div>