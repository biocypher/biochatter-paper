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
  <meta name="dc.modified" content="2023-10-27T09:46:28+00:00" />
  <meta property="article:modified_time" content="2023-10-27T09:46:28+00:00" />
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
  <link rel="alternate" type="text/html" href="https://biocypher.github.io/biochatter-paper/v/7c327ac4fefa581c888b4bbb9710dfaf7f0562cf/" />
  <meta name="manubot_html_url_versioned" content="https://biocypher.github.io/biochatter-paper/v/7c327ac4fefa581c888b4bbb9710dfaf7f0562cf/" />
  <meta name="manubot_pdf_url_versioned" content="https://biocypher.github.io/biochatter-paper/v/7c327ac4fefa581c888b4bbb9710dfaf7f0562cf/manuscript.pdf" />
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
([permalink](https://biocypher.github.io/biochatter-paper/v/7c327ac4fefa581c888b4bbb9710dfaf7f0562cf/))
was automatically generated
from [biocypher/biochatter-paper@7c327ac](https://github.com/biocypher/biochatter-paper/tree/7c327ac4fefa581c888b4bbb9710dfaf7f0562cf)
on October 27, 2023.
</em></small>



## Authors



+ **Sebastian Lobentanzer**
  ^[✉](#correspondence)^<br>
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
  ^[✉](#correspondence)^<br>
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
or email to
Sebastian Lobentanzer \<sebastian.lobentanzer@gmail.com\>, 
Julio Saez-Rodriguez \<pub.saez@uni-heidelberg.de\>.


:::


## Abstract {.page_break_before}

The wealth of knowledge we have amassed in the context of biomedical science has grown exponentially in the last decades.
Consequently, understanding and contextualising scientific results has become increasingly difficult for any single individual.
In contrast, current Large Language Models (LLMs) can remember an enormous amount of information, but have notable shortcomings, such as a lack of generalised awareness, logical deficits, and a propensity to hallucinate.
To improve biomedical analyses, we propose to combine human ingenuity and machine memory by means of an open and modular conversational platform, [biochatter](https://github.com/biocypher/biochatter), exemplified in the web application [ChatGSE](https://chat.biocypher.org).
We safeguard against common LLM shortcomings using general and biomedicine-specific measures and allow automated integration of popular bioinformatics methods.
Ultimately, we aim to improve the AI-readiness of biomedicine and make LLMs more useful and trustworthy in research applications.


## Main

Despite our technological advances, biology and biomedicine continue to pose incredible challenges [@{https://www.bbc.com/news/health-65252510}].
We measure more and more data points with ever-increasing resolution to such a degree that their analysis and interpretation have become the bottleneck for their exploitation.
One reason for this challenge may be the inherent limitation of human knowledge [@doi:10.1016/j.tics.2005.04.010].
Even seasoned domain experts cannot know the implications of every molecule, be it metabolite, DNA, RNA, or protein, even in their own domain.
In addition, biological events are context-dependent, for instance with respect to a cell type or specific disease.

Large Language Models (LLMs) of the current generation, on the other hand, can access enormous amounts of knowledge, encoded (incomprehensibly) in their billions of parameters [@doi:10.48550/arxiv.2204.02311, @10.48550/arxiv.2201.08239, @10.48550/arxiv.2303.08774].
Trained correctly, they can recall and combine virtually limitless knowledge from their training set.
ChatGPT has taken the world by storm, and many biomedical researchers already use LLMs in their daily work, for general as well as bioinformatics-specific tasks [@doi:10.1101/2023.04.16.537094, @doi:10.1038/s41587-023-01789-6].
However, the current, predominantly manual, way of interacting with LLMs is virtually non-reproducible, and their behaviour can be erratic.
For instance, they are known to hallucinate: they make up facts as they go along, and, to make matters worse, are convinced - and convincing - regarding the truth of their hallucinations [@doi:10.1038/s41586-023-05881-4, @doi:10.1038/s41587-023-01789-6].
While current efforts towards AGI (Artificial General Intelligence) manage to ameliorate some of the shortcomings by ensembling multiple models [@{https://python.langchain.com}] with long-term memory stores [@{https://autogpt.net/}], the current generation of AI does not inspire adequate trust to be applied to biomedical problems without supervision [@doi:10.1038/s41586-023-05881-4].
Additionally, biomedicine demands greater care in data privacy, licensing, and transparency than most other real-world issues.

A major aim of computational biology is to distil high-dimensional molecular measurements into a humanly digestible form by projecting the measurements into a lower-dimensional space composed of gene programs, pathways, or other functional groupings of biological entities, for example via gene set enrichment analyses.
However, even this distilled knowledge requires advanced expertise and thorough literature research to effectively interpret and exploit, and benchmarking the methods’ performance is non-trivial [@doi:10.1093/bib/bbz158].

To improve and accelerate this interpretation and exploration, we have developed biochatter, a platform for communicating with LLMs specifically tuned to biomedical research, the use of which we demonstrate in a conversational web interface, ChatGSE (Figure @fig:overview).
The platform guides the human researcher intuitively through the interaction with the model, while counteracting the problematic behaviours of the LLM.
Since the interaction is mainly based on plain text, it can be used by virtually any researcher.
We engineer prompts around the queries of the user to improve model performance with regard to biomedicine, and automate the integration of popular bioinformatics methods, such as differential expression and gene set enrichment (Supplementary Note [Prompt Engineering]).

<!-- Figure 1 -->
![
**The ChatGSE composable platform architecture (simplified).**
The user submits a question about a topic of interest (e.g., an experiment) along with the low-dimensional results of a bioinformatics analysis (top left).
The platform’s main response circuit (blue) composes a number of specifically engineered prompts and passes them (and a conversation history) to the primary LLM, which generates a response for the user based on all inputs.
This response is simultaneously used to prompt the secondary circuit (orange), which fulfils auxiliary tasks to complement the primary response.
In particular, using search, the secondary circuit queries a database as prior knowledge repository and compares annotations to the primary response.
The knowledge graph can also serve as long-term memory extension of the model.
Further, an independent LLM receives the primary response for fact-checking, which can be supplemented with context-specific information by a document summarisation model.
If this “second opinion” differs from the primary response, a warning is issued.
The platform is composable in all aspects, in principle allowing arbitrary extensions to other, specialised models for additional tasks orchestrated by the primary LLM.
](images/graphical_abstract.png "Overview"){#fig:overview}

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>


## Supplementary Materials

In our Supplementary Notes, we explain the functions of our platform in more detail.
Please note that several of the mentioned features, particularly more advanced ones, are in early developmental stages.
For practical reasons, we divide our software into two distinct packages, the user interface (UI) component [ChatGSE](https://github.com/biocypher/ChatGSE) and the Python backend library [biochatter](https://github.com/biocypher/biochatter).
This also reflects how we expect the platform to be used: as a generic backend library for the development of custom UIs.
For an up-to-date overview and preview of current functionality of the platform, please visit the [online preview](https://chat.biocypher.org).
Both libraries are developed in Python (version 3.10), according to modern standards of software development [@doi:10.1038/s41597-020-0486-7].
We use Streamlit (version 1.21.0, https://streamlit.io) for the web UI.
We include a code of conduct and contributor guidelines to offer accessibility and inclusivity to all that are interested in contributing to the framework.

### Prompt Engineering
