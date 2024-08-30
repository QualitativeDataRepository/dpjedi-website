---
title: Markdown Test Page
permalink: /test/
layout: markdown
toc: true
---

# {{ page.title }}

## General

### Sample Table

<!-- Include the table -->
<!-- <pre>{{ page.table_data | jsonify }}</pre> -->
<!-- {{ page.table_data | inspect }} -->
{% capture table_headers %}
Column 1, Column 2, Column 3
{% endcapture %}

{% capture table_rows %}
Row 1, Cell 1 | Row 1, Cell 2 | Row 1, Cell 3
Row 2, Cell 1 | Row 2, Cell 2 | Row 2, Cell 3
Row 3, Cell 1 | Row 3, Cell 2 | Row 3, Cell 3
{% endcapture %}

{% assign headers_array = table_headers | split: ', ' %}
{% assign rows_array = table_rows | newline_to_br | split: '<br />' %}

{% include table.html headers=headers_array rows=rows_array %}

Publishers often offer guidelines and associated resources relating to editorial practices. While typically provided for editors of the journals that they publish, these resources may also be more generally helpful. For some examples, see:

- [PLOS ONE](https://journals.plos.org/plosone/s/resources-for-editors)
- [SAGE](https://us.sagepub.com/en-us/nam/resources-journal-authors-and-editors)
- [Springer](https://www.springer.com/gp/authors-editors/editors)
- [Taylor and Francis](https://editorresources.taylorandfrancis.com/)
- [Wiley](https://authorservices.wiley.com/editors/index.html)

## Incoming Editors

If you are just starting out as a journal editor, you might find the [Committee on Publication Ethics’](https://publicationethics.org/) short [guide to ethical editing for new editors](https://publicationethics.org/resources/guidelines-new/short-guide-ethical-editing-new-editors) helpful, as well as this [glossary of publishing and editing terms](https://www.pauldudenhefer.net/glossary-of-publishing-and-editing-terms).

The [PKP school](https://pkpschool.sfu.ca/about/) also offers a [free course in becoming an editor](https://pkpschool.sfu.ca/courses/becoming-an-editor/), focusing on how to perform the major tasks required of an editor for a scholarly journal, how to analyze and solve common problems that may arise when editing a scholarly journal, how to assist other members of the journal team, and where to look for help with difficult issues.

The [Council of Science Editors](https://www.councilscienceeditors.org/) has [sample correspondence for an editorial office](https://www.councilscienceeditors.org/resource-library/editorial-policies/sample-correspondence-for-an-editorial-office/) that you can customize to suit your journal, and also offers [short courses in journal and manuscript editing](https://www.councilscienceeditors.org/resource-library/cse-short-course-descriptions/). The [European Association of Science Editors (EASE)](https://ease.org.uk/) offers training and webinars, a [Science Editors' Handbook](https://ease.org.uk/publications/science-editors-handbook/) and a [guide on how to select reviewers](https://ease.org.uk/communities/peer-review-committee/peer-review-toolkit/how-to-select-reviewers/). EASE also offers [Editorial School for Journal Editors](https://ease.org.uk/ease-events/training/editorial-school-for-journal-editors/), a four-week course on a range of topics relevant to editing.

The process of onboarding associate/action editors will vary hugely across journals. Most journals will provide at least some guidelines, whether written or otherwise (e.g., see this [video introduction](https://www.youtube.com/watch?v=3eTA2YkzqFc) for editors and reviewers at *Collabra: Psychology*). Journals may also offer opportunities for incoming editors to reassure themselves that they have comprehended these guidelines. [PCI Registered Reports](https://rr.peercommunityin.org/about/about) does this (see their [guide](https://rr.peercommunityin.org/help/guide_for_recommenders#h_177144648851613645297185) and [test](https://docs.google.com/forms/d/e/1FAIpQLSdoEQ3cfWdDmRixeq8oGUoTN-bVtcdOtriOVDveDMg3bULAeQ/viewform)), as well as *Collabra* (see their [editing training guide](https://docs.google.com/presentation/d/1zzEItmrMQpA3stKTL2X4Sl1XFCq6Qbi1uTYEwHb6-zE/edit#slide=id.g1acac551868_0_119) and the [associated test](https://docs.google.com/forms/d/e/1FAIpQLSc73GmDVYXZOHCewcm17KA_IKNHaXmgK-LT29SEeUCoQjoJXA/viewform)).

Publishers will sometimes have resources relevant to editing, including [Springer Nature](https://www.springernature.com/gp/editors/editor-courses), and [Elsevier](https://researcheracademy.elsevier.com/editor-essentials/editor-essentials).

## Ethics

The [Committee on Publication Ethics](https://publicationethics.org/) has many resources to help journal editors deal with ethical issues, including guidelines and case studies. For example, they have [guidelines on publication manipulation](https://publicationethics.org/files/Systematic_manipulation_of_the_publication_process.pdf).

The [Council of Science Editors](https://www.councilscienceeditors.org/) has a [white paper on publication ethics](https://www.councilscienceeditors.org/resource-library/editorial-policies/white-paper-on-publication-ethics/) including a guide to [editor roles and responsibilities](https://www.councilscienceeditors.org/resource-library/editorial-policies/white-paper-on-publication-ethics/2-1-editor-roles-and-responsibilities/).

Although some ethical issues are clearly defined (e.g. that authors should not fabricate data), there are other areas where there is debate surrounding the lines of editorial responsibility. For example, [*Nature Human Behavior*](https://www.nature.com/nathumbehav/) has put in place a [new research ethics policy](https://www.nature.com/nature-portfolio/editorial-policies/ethics-and-biosecurity) that addresses potential harms for human population groups who do not participate in research but may be harmed by its publication ([see the editorial introducing the policy here](https://www.nature.com/articles/s41562-022-01443-2)). However, there have been some criticisms of the policy, suggesting that its vagueness could be open to abuse and stand in the way of “truth”. For one discussion on whether and how (identity- and ideological-based) diversity and scientific values should impact the research that gets conducted and published in psychology see [Conry-Murray & Silverstein (2022)](https://doi.org/10.31234/osf.io/cskg2).

### Editors publishing in their own journals

There is some controversy surrounding the question of whether editors should be allowed to publish in the journals that they edit. Where this is permitted, journals should have clear processes in place to evaluate articles submitted by editors to their own journals.

[Helgesson et al. (2022)](https://doi.org/10.1002/leap.1449) conducted a systematic review of the prevalence of this practice. They found large variability of self-publishing across fields, journals, and editors, but ultimately that there are some situations where levels of self-publication are very high. This is corroborated by [Bishop (2020)](http://deevybee.blogspot.com/2020/08/pepiops-prolific-editors-who-publish-in.html) who found that there are even some cases where the most prolific author in a journal is the editor-in-chief! In addition, among biomedical journals where few authors were responsible for a disproportionate number of publications, the most prolific author was part of the editorial board in over 60% of cases ([Scanff et al., 2021](https://doi.org/10.1371/journal.pbio.3001525)).

## Diversifying Social Science Research

An argument can be made that social science disciplines are characterized by different kinds of systemic inequality. For example, elitism is one source of inequality – [Kawa et al. (2019)](https://doi.org/10.1111/aman.13158) found that the top 5 or so anthropology departments in the USA all hire each others' graduates. Another example is authors’ limited geographical distribution. Of the authors who published articles in the top five developmental psychology journals between 2006 and 2010, fewer than 3% were from countries in Central or South America, Africa, Asia, or the Middle East ([Nielsen et al., 2017](https://doi-org.libezproxy2.syr.edu/10.1016/j.jecp.2017.04.017)). This limitation also extends to journal editors ([Altman & Cohen, 2021](http://www.doi.org/10.31235/osf.io/4nq97)). This is reflected in citation patterns too – [this article](https://www.insidehighered.com/advice/2021/08/27/entrenched-inequity-not-appropriately-citing-scholarship-women-and-people-color) points to the trend of inadequately citing or omitting scholarship by women and people of color and suggests some best practices journals can adopt to avoid this.

Some fields have developed local resources that could be adapted to other fields. For example, [Roberts et al. (2020)](https://doi.org/10.1177/1745691620927709) examine racial inequality in psychological research to date and offer recommendations for editors and authors for working towards research that benefits from diversity in editing, writing, and participation. [Buchanan et al. (2020)](https://doi.org/10.31234/osf.io/6nk4x) also discuss strategies for upending racism in psychological science. In a different paper, [Buchanan et al. (2021)](https://doi.org/10.31234/osf.io/zp9em) propose a Diversity Accountability Index for Journals (DAI-J) in order to increase awareness and establish accountability across psychology journals. The [American Psychological Association](https://www.apa.org/) also offers some general tips and resources on [building diversity in the field](https://www.apa.org/about/apa/equity-diversity-inclusion/publications/editorial-board-members). [Dixon et al. (2023)](https://doi.org/10.31234/osf.io/5me2z) find that such special issues and increased diversity among editorial boards are a necessary first step, but more work is needed to ensure their success.

For an example of a practical guide for reforming inequalities in a different field, see [Taffe & Gilpin (2021)](https://doi.org/10.1152/ajpendo.00330.2020).

## Open Science

Open science is a set of principles and practices designed to increase the transparency and replicability of science and encourage the availability and reuse of scientific data. Journals are encouraged to develop policies that promote open science, including policies on data sharing, pre-registration, and open access. The [Transparency and Openness Promotion (TOP)](https://www.cos.io/initiatives/top-guidelines) guidelines provide a set of standards for promoting open science, which journals can adopt.

The [Center for Open Science (COS)](https://www.cos.io/) offers [resources for editors and reviewers](https://www.cos.io/editors-and-reviewers) to help them promote open science in their journals. COS also offers [free Open Science badges](https://www.cos.io/initiatives/badges), which journals can award to articles that meet certain standards of transparency and openness.

## Peer Review

The peer review process is a key part of scholarly publishing, but it is also one of the most controversial. Journals have different policies on peer review, including whether it is single-blind, double-blind, or open. The [COPE Ethical Guidelines for Peer Reviewers](https://publicationethics.org/resources/guidelines-new/cope-ethical-guidelines-peer-reviewers) provide a set of standards for ethical peer review.

The [Peer Review Toolkit](https://peerreview.ac.uk/) offers a range of resources for editors, including guidelines on how to select and work with reviewers, how to handle conflicts of interest, and how to ensure that peer review is fair and unbiased. The toolkit is developed by [Sense about Science](https://www.senseaboutscience.org/), a UK-based charity that promotes evidence-based science and public engagement.

The [Peer Review Congress](https://peerreviewcongress.org/) is a biennial conference that brings together editors, reviewers, and researchers to discuss the latest developments in peer review. The conference is organized by the [International Society of Managing and Technical Editors (ISMTE)](https://www.ismte.org/), which also offers training and resources for editors.

## The Journal Editing Workflow

Different journals will have different workflows for handling submissions, peer review, and publication. However, there are some general principles that apply to most journals. The [COPE](https://publicationethics.org/) and [ISMTE](https://www.ismte.org/) both offer resources on best practices for managing the editorial workflow.

The [Elsevier Journal Manager's Handbook](https://www.elsevier.com/editors/journal-managers-handbook) provides a detailed guide to the different stages of the journal editing process, from submission to publication. The handbook includes advice on how to manage the peer review process, how to handle ethical issues, and how to work with authors and reviewers.

## Specific Challenges

Journals may also face specific challenges, such as handling large volumes of submissions, dealing with controversial research, or managing conflicts of interest. The [COPE](https://publicationethics.org/) offers a range of resources to help editors deal with these challenges, including case studies, guidelines, and best practice recommendations.