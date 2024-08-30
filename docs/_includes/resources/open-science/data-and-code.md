### Data and Code

A set of stable core practices has begun to emerge with regard to data management and sharing. While all are readily available, some require more effort on the part of journals. For example, requiring authors to share data via a trusted digital repository (and not e.g., via a personal website) is easier than checking that the author's code runs. Iain Hrynaszkiewicz (*[Public Library of Science](https://plos.org/)* (PLOS)) has written a chapter outlining “[Publishers’ Responsibilities in Promoting Data Quality and Reproducibility](https://doi.org/10.1007/164_2019_290)” that describes practical approaches being taken by publishers to promote rigor and transparency in data practices.

Journals are increasingly adopting data and code availability policies. The [Research Data Alliance](https://rd-alliance.org/) has developed a [Research Data Policy Framework](https://datascience.codata.org/article/10.5334/dsj-2020-005/) for all journals and publishers including template policy texts which can be implemented by journals in their Information for Authors and publishing workflows.

There are many repositories to choose from, and different repositories will have benefits for different fields and needs. For lists of recommended repositories, see for example: [section 2.2.1 in *F1000 Research*’s data guidelines](https://f1000research.com/for-authors/data-guidelines); [Springer Nature’s list of social science repository examples](https://www.springernature.com/gp/authors/research-data-policy/repositories-socsci/12327116); and [*PLOS One*’s recommended repositories](https://journals.plos.org/plosone/s/recommended-repositories). Similarly, the *[Society for Social and Personality Psychology](https://www.spsp.org/publications/guidelines-resources#4)* has created a matrix of different trusted repositories and what they offer. Similarly, [re3data](https://www.re3data.org/browse/by-subject/) provides a database of different repositories and their attributes categorized by subject, content type, and country.

[Goodman et al. (2014)](https://doi.org/10.1371/journal.pcbi.1003542) states that “A proper, trustworthy archive will: (1) assign an identifier such as a “handle” (hdl) or “digital object identifier” (doi) (see the [DOI handbook](https://www.doi.org/doi_handbook/6_Policies.html#6.5)); (2) require that you provide adequate documentation and metadata; and (3) manage the “care and feeding” of your data by employing good curation practices”. The [Research Data Alliance](https://www.rd-alliance.org/) have created [10 Things for Curating Reproducible and FAIR Research](https://www.rd-alliance.org/group/cure-fair-wg/outcomes/10-things-curating-reproducible-and-fair-research) and [The CoreTrustSeal Trustworthy Data Repositories Requirements](https://doi.org/10.5281/zenodo.3638211). See also the [FAIR Guiding Principles](https://www.go-fair.org/fair-principles/) for data management and stewardship.

In some fields (e.g., economics), it is common practice to have on the editorial team a specific “data editor”. These data editors are responsible for creating, adapting, and implementing data and code sharing policies at their respective journals. Data editors often share important information that can be useful for other editors looking to adopt or adapt their existing data and code sharing policies. For example, the data editor websites for the *[American Economic Association](https://aeadataeditor.github.io/)*, *[The Review of Economic Studies](https://restud.github.io/data-editor/)*, and *[The Economic Journal](https://ejdataeditor.github.io/)* all offer a wealth of information and advice. See, for example, the *[American Economic Association](https://aeadataeditor.github.io/)* policy on [revisions of data and code deposits](https://www.aeaweb.org/journals/data/policy-revisions) in the AEA data and code repository.

#### Data Ethics

It is important to note that there will be cases where data cannot be shared, and that it is important to be “as open as possible, as closed as necessary”. See [Meyer (2018)](https://doi.org/10.1177/2515245917747656) for an excellent guide on “ethical data sharing”. GREI (the NIH Generalist Repository Ecosystem Initiative) also has [a webinar series](https://datascience.nih.gov/grei-collaborative-webinar-series) on this topic.

[FORCE11](https://www.force11.org/) and [COPE](https://publicationethics.org/) have developed some recommendations for the handling of ethical concerns relating to the publication of research data. See their [blog post](https://www.force11.org/article/recommendations-handling-ethical-concerns-relating-publication-research-data) and the [recommendations](https://zenodo.org/record/5391293#.YYATD9bP0-Q) themselves here.

There may be particular types of data that are more difficult to share – e.g., data on sensitive topics. For a case study that includes challenges, tools, and future directions of sharing data in these cases, please see [Joel et al. (2018)](https://doi.org/10.1177%2F2515245917744281). For a case study that discusses the redaction of sensitive data, see [Casadevall et al. (2013)](https://doi.org/10.1128/mBio.00991-13). Many repositories offer restricted access to data, e.g., the repositories organized in [Data-PASS](http://www.data-pass.org) (e.g., [ICPSR](https://www.icpsr.umich.edu/web/pages/), [QDR](https://qdr.syr.edu/), [Odum](https://odum.unc.edu/archive/), [Databrary](https://nyu.databrary.org/)), and almost all repositories organized in [CESSDA](https://www.cessda.eu/).

#### Open Data

Mandating or encouraging authors to share data alongside their manuscripts means that reviewers (and later, readers) can:

- See the structure of the data more clearly
- Run additional analyses
- Use the data to answer new questions

In addition, there may be a citation advantage for authors sharing data ([Colavizza et al., 2020](https://doi.org/10.1371/journal.pone.0230416)).

#### Open Code

Mandating or encouraging authors to share code alongside their manuscripts means that reviewers (and later, readers) can:

- See the analyses that were conducted more clearly
- Check whether the code runs on another (similarly structured) dataset

Authors can also give reviewers the opportunity to check basic code functionality by providing synthetic data. Dan Quintana has done a lot of work promoting the sharing of synthetic datasets and providing resources to help authors do so – see his [YouTube video](https://bit.ly/3mjx088), [blog post](https://www.dsquintana.blog/creating-and-synthetic-version-of-a-real-dataset/), and [Quintana (2020)](http://doi.org/10.7554/eLife.53275).

#### Open Data and Code

Mandating or encouraging authors to share both data and code alongside their manuscripts has all the above benefits of sharing either of these separately, but also means that reviewers (and later, readers) can check the computational reproducibility of the results (i.e., does running the code on the data produce the same results that are reported in the paper).

The *[American Economic Association](https://www.aeaweb.org/)* provides helpful [guidance on implementation of their data and code availability policy](https://aeadataeditor.github.io/aea-de-guidance/) that could easily be applied to other journals and fields. [The Berkeley Institute for Transparency in the Social Sciences](https://www.bitss.org/) offers a handy [guide on conducting reproducibility checks](https://bitss.github.io/ACRE/).

For a discussion of the impact of journal data policy strictness on the code re-execution rate (i.e., how likely the code is to run without errors) and a set of recommendations for code dissemination aimed at journals, see [Trisovic et al. (2020)](https://arxiv.org/abs/2103.12793).

#### Pre-publication Verification of Analyses

Some journals have now adopted a policy whereby data and code are not only required for publication in the journal, but must be checked before publication to ensure that the analyses are reproducible – that the results in the manuscript match the results that are produced when someone who is not one of the authors re-runs the code on the data. This is called pre-publication “verification of analyses”, “data and code replication”, or “reproduction of analyses”. See [Willis & Stodden (2020)](https://doi.org/10.1162/99608f92.25982dcf) for a useful overview of how to leverage policies, workflows, and infrastructure to ensure computational reproducibility in publication.

For more information on how to implement a policy like this at your journal, see the [Data and Code Guidance by Data Editors](https://social-science-data-editors.github.io/guidance/) developed by Lars Vilhuber and colleagues, which is used by the *[American Economic Association](https://www.aeaweb.org/journals)* journals, *[Canadian Journal of Economics](https://onlinelibrary.wiley.com/journal/15405982)*, the *[Review of Economic Studies](https://academic.oup.com/restud)*, and the *[Economic Journal](https://academic.oup.com/ej)* as a reference. This [practical guide on training students to assess the reproducibility of articles in the social sciences](https://labordynamicsinstitute.github.io/ldilab-manual/index.html) may also be of interest.

Several journals in political science also require pre-publication verification. See for example *[State Politics & Policy Quarterly](https://www.cambridge.org/core/journals/state-politics-and-policy-quarterly/information/instructions-contributors)*, *[Political Analysis](https://www.cambridge.org/core/journals/political-analysis/information/instructions-contributors)*, and the *[American Journal of Political Science](https://ajps.org/)*.

#### Resources for Open Research Planning & Documentation

Many platforms can aid researchers in making their entire workflows open and transparent. Here are a few examples:

- [Code Ocean](http://codeocean.com/)
- [The Whole Tale](http://wholetale.org/)
- [Authorea](https://www.authorea.com/product)
- [RSpace](https://www.researchspace.com/)
- [Research Equals](https://libscie.org/researchequals-com/)

#### Data Citation

The social sciences are increasingly adopting the use of permanent identifiers, such as digital object identifiers (DOIs), for datasets, making it easier to find and cite data sources. There may be additional stylistic guidelines that are discipline-specific, for example, this [guide to dataset references](https://apastyle.apa.org/style-grammar-guidelines/references/examples/data-set-references) from the *[American Psychological Association](https://apastyle.apa.org/)*.

Many guides for data citation exist that can be shared with authors and/or adopted as a policy at your journal:

- [TOP Guidelines](https://www.cos.io/initiatives/top-guidelines) (section on Citation Standards)
- [Joint Declaration of Data Citation Principles](https://doi.org/10.25490/a97f-egyk)
- [Guidance on Data Citations](https://social-science-data-editors.github.io/guidance/addtl-data-citation-guidance.html#many-related-datasets) (including a [widget for computing citations](https://social-science-data-editors.github.io/guidance/addtl-data-citation-guidance.html#try-it-out))
- [DataCite](https://datacite.org/) (including [DataCite Metadata Schema](https://schema.datacite.org/))
- [How to Cite Data and Statistics](https://guides.nyu.edu/datasources/data-citation)
- [Citing data sources – Why is it good and how to do it?](https://library.cumc.columbia.edu/insight/citing-data-sources)

[DataSeer](https://dataseer.ai/) is intended to help journals flag references to data in manuscripts, which could be used to ensure all data referenced are being properly cited.

#### Heterogeneous Data and Analytic Materials

While this section is framed in terms of numeric data and computer code, it is worth noting that cognate considerations arise in all circumstances where authors use a combination of data and analytic reasoning to make their findings. For example, authors can also make qualitative data and materials available for case studies that used process tracing analyses and relied on interviews and archival data.
