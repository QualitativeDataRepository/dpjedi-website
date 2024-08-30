{% capture list_items %}
November 15 and 16, 2023 | JEDI 2023 Annual Meeting: Improving Published Research [JEDI 2023 Annual Meeting: Improving Published Research]({{ site.baseurl }}/events/jedi-2023-annual-meeting)
 | Panel 1: Experiences with correcting the scientific record [Panel 1: Experiences with correcting the scientific record]({{ site.baseurl }}/events/jedi-2023-annual-meeting#panel1)
 | Panel 2: Transparency in peer review: challenges and opportunities [Panel 2: Transparency in peer review: challenges and opportunities]({{ site.baseurl }}/events/jedi-2023-annual-meeting#panel2)
Friday, May 20, 2022 | May the force be with you: Resources to help journal editors advance their fields [Agenda, slides, and recordings]({{ site.baseurl }}/events/may-the-force-be-with-you)
Friday, November 20, 2020 | As Open as Possible, As Closed as Necessary: Empowering Transparency in Publications Based on Sensitive Research Data [Agenda, slides, and recordings]({{ site.baseurl }}/events/as-open-as-possible)
{% endcapture %}

{% assign items_array = list_items | newline_to_br | split: '<br />' %}

{% include listgroup-custom.html items=items_array %}