---
title: A Platform for the Biomedical Application of Large Language Models
keywords:
- biomedicine
- bioinformatics
- large language models
- framework
lang: en-UK
date-meta: '2023-10-27'
author-meta:
- Sebastian Lobentanzer
- Julio Saez-Rodriguez
header-includes: |
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta property="og:type" content="article" />
  <meta name="dc.title" content="A Platform for the Biomedical Application of Large Language Models" />
  <meta name="citation_title" content="A Platform for the Biomedical Application of Large Language Models" />
  <meta property="og:title" content="A Platform for the Biomedical Application of Large Language Models" />
  <meta property="twitter:title" content="A Platform for the Biomedical Application of Large Language Models" />
  <meta name="dc.date" content="2023-10-27" />
  <meta name="citation_publication_date" content="2023-10-27" />
  <meta property="article:published_time" content="2023-10-27" />
  <meta name="dc.modified" content="2023-10-27T08:18:20+00:00" />
  <meta property="article:modified_time" content="2023-10-27T08:18:20+00:00" />
  <meta name="dc.language" content="en-UK" />
  <meta name="citation_language" content="en-UK" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="Sebastian Lobentanzer" />
  <meta name="citation_author_institution" content="Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany" />
  <meta name="citation_author_orcid" content="0000-0003-3399-6695" />
  <meta name="twitter:creator" content="@slobentanzer" />
  <meta name="citation_author" content="Julio Saez-Rodriguez" />
  <meta name="citation_author_institution" content="Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany" />
  <meta name="citation_author_orcid" content="0000-0002-8552-8976" />
  <meta name="twitter:creator" content="@saezlab" />
  <link rel="canonical" href="https://biocypher.github.io/biochatter-paper/" />
  <meta property="og:url" content="https://biocypher.github.io/biochatter-paper/" />
  <meta property="twitter:url" content="https://biocypher.github.io/biochatter-paper/" />
  <meta name="citation_fulltext_html_url" content="https://biocypher.github.io/biochatter-paper/" />
  <meta name="citation_pdf_url" content="https://biocypher.github.io/biochatter-paper/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://biocypher.github.io/biochatter-paper/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://biocypher.github.io/biochatter-paper/v/fa69d7a71e35f621b0ae36f86a354120658dd4a3/" />
  <meta name="manubot_html_url_versioned" content="https://biocypher.github.io/biochatter-paper/v/fa69d7a71e35f621b0ae36f86a354120658dd4a3/" />
  <meta name="manubot_pdf_url_versioned" content="https://biocypher.github.io/biochatter-paper/v/fa69d7a71e35f621b0ae36f86a354120658dd4a3/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://biocypher.github.io/biochatter-paper/v/fa69d7a71e35f621b0ae36f86a354120658dd4a3/))
was automatically generated
from [biocypher/biochatter-paper@fa69d7a](https://github.com/biocypher/biochatter-paper/tree/fa69d7a71e35f621b0ae36f86a354120658dd4a3)
on October 27, 2023.
</em></small>



## Authors



+ **Sebastian Lobentanzer**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0003-3399-6695](https://orcid.org/0000-0003-3399-6695)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [slobentanzer](https://github.com/slobentanzer)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [slobentanzer](https://twitter.com/slobentanzer)
    <br>
  <small>
     Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany
  </small>

+ **Julio Saez-Rodriguez**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-8552-8976](https://orcid.org/0000-0002-8552-8976)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [saezrodriguez](https://github.com/saezrodriguez)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [saezlab](https://twitter.com/saezlab)
    <br>
  <small>
     Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany
  </small>


::: {#correspondence}
✉ — Correspondence possible via [GitHub Issues](https://github.com/biocypher/biochatter-paper/issues)

:::


## Abstract {.page_break_before}

The wealth of knowledge we have amassed in the context of biomedical science has grown exponentially in the last decades.
Consequently, understanding and contextualising scientific results has become increasingly difficult for any single individual.
In contrast, current Large Language Models (LLMs) can remember an enormous amount of information, but have notable shortcomings, such as a lack of generalised awareness, logical deficits, and a propensity to hallucinate.
To improve biomedical analyses, we propose to combine human ingenuity and machine memory by means of an open and modular conversational platform, [biochatter](https://github.com/biocypher/biochatter), exemplified in the web application [ChatGSE](https://chat.biocypher.org).
We safeguard against common LLM shortcomings using general and biomedicine-specific measures and allow automated integration of popular bioinformatics methods.
Ultimately, we aim to improve the AI-readiness of biomedicine and make LLMs more useful and trustworthy in research applications.


## Main

Despite our technological advances, biology and biomedicine continue to pose incredible challenges (Gallagher, 2023).
We measure more and more data points with ever-increasing resolution to such a degree that their analysis and interpretation have become the bottleneck for their exploitation.
One reason for this challenge may be the inherent limitation of human knowledge (Marois and Ivanoff, 2005).
Even seasoned domain experts cannot know the implications of every molecule, be it metabolite, DNA, RNA, or protein, even in their own domain.
In addition, biological events are context-dependent, for instance with respect to a cell type or specific disease.

Citation by URL [@{https://www.bbc.com/news/health-65252510}].

Citation by alias [@gallagher-infinite].

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>

