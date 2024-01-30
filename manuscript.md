---
title: A Platform for the Biomedical Application of Large Language Models
keywords:
- biomedicine
- large language models
- framework
- retrieval-augmented generation
- knowledge graph
lang: en-UK
date-meta: '2024-01-30'
author-meta:
- Sebastian Lobentanzer
- Shaohong Feng
- The BioChatter Consortium
- Andreas Maier
- Cankun Wang
- Nils Krehl
- Qin Ma
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
  <meta name="dc.date" content="2024-01-30" />
  <meta name="citation_publication_date" content="2024-01-30" />
  <meta property="article:published_time" content="2024-01-30" />
  <meta name="dc.modified" content="2024-01-30T15:07:08+00:00" />
  <meta property="article:modified_time" content="2024-01-30T15:07:08+00:00" />
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
  <meta name="citation_author" content="Shaohong Feng" />
  <meta name="citation_author_institution" content="Department of Biomedical Informatics, The Ohio State University, Columbus, Ohio, USA" />
  <meta name="citation_author_orcid" content="0009-0000-8124-3626" />
  <meta name="citation_author" content="The BioChatter Consortium" />
  <meta name="citation_author" content="Andreas Maier" />
  <meta name="citation_author_institution" content="Institute for Computational Systems Biology, University of Hamburg, Hamburg, Germany" />
  <meta name="citation_author_orcid" content="0000-0003-4408-0068" />
  <meta name="citation_author" content="Cankun Wang" />
  <meta name="citation_author_institution" content="Department of Biomedical Informatics, The Ohio State University, Columbus, Ohio, USA" />
  <meta name="citation_author_orcid" content="0000-0002-0225-9855" />
  <meta name="twitter:creator" content="@Wang-Cankun" />
  <meta name="citation_author" content="Nils Krehl" />
  <meta name="citation_author_institution" content="Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany" />
  <meta name="citation_author_orcid" content="TBD" />
  <meta name="citation_author" content="Qin Ma" />
  <meta name="citation_author_institution" content="Department of Biomedical Informatics, The Ohio State University, Columbus, Ohio, USA" />
  <meta name="citation_author_orcid" content="0000-0002-3264-8392" />
  <meta name="twitter:creator" content="@QinMaBMBL" />
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
  <link rel="alternate" type="text/html" href="https://biocypher.github.io/biochatter-paper/v/747ebc72d4dc890000a47e0e077c78f6548a71d9/" />
  <meta name="manubot_html_url_versioned" content="https://biocypher.github.io/biochatter-paper/v/747ebc72d4dc890000a47e0e077c78f6548a71d9/" />
  <meta name="manubot_pdf_url_versioned" content="https://biocypher.github.io/biochatter-paper/v/747ebc72d4dc890000a47e0e077c78f6548a71d9/manuscript.pdf" />
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
([permalink](https://biocypher.github.io/biochatter-paper/v/747ebc72d4dc890000a47e0e077c78f6548a71d9/))
was automatically generated
from [biocypher/biochatter-paper@747ebc7](https://github.com/biocypher/biochatter-paper/tree/747ebc72d4dc890000a47e0e077c78f6548a71d9)
on January 30, 2024.
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

+ **Shaohong Feng**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0009-0000-8124-3626](https://orcid.org/0009-0000-8124-3626)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [fengsh27](https://github.com/fengsh27)
    <br>
  <small>
     Department of Biomedical Informatics, The Ohio State University, Columbus, Ohio, USA
  </small>

+ **The BioChatter Consortium**
  <br>
  <small>
  </small>

+ **Andreas Maier**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0003-4408-0068](https://orcid.org/0000-0003-4408-0068)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [andimajore](https://github.com/andimajore)
    <br>
  <small>
     Institute for Computational Systems Biology, University of Hamburg, Hamburg, Germany
  </small>

+ **Cankun Wang**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-0225-9855](https://orcid.org/0000-0002-0225-9855)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [Wang-Cankun](https://github.com/Wang-Cankun)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [Wang-Cankun](https://twitter.com/Wang-Cankun)
    <br>
  <small>
     Department of Biomedical Informatics, The Ohio State University, Columbus, Ohio, USA
  </small>

+ **Nils Krehl**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [TBD](https://orcid.org/TBD)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [nilskre](https://github.com/nilskre)
    <br>
  <small>
     Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany
  </small>

+ **Qin Ma**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-3264-8392](https://orcid.org/0000-0002-3264-8392)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [maqin2001](https://github.com/maqin2001)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [QinMaBMBL](https://twitter.com/QinMaBMBL)
    <br>
  <small>
     Department of Biomedical Informatics, The Ohio State University, Columbus, Ohio, USA
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

Authors between consortium and last author are ordered alphabetically.

## Abstract {.page_break_before}

Current-generation Large Language Models (LLMs) have stirred enormous interest in the recent months, yielding great potential for accessibility and automation, while simultaneously posing significant challenges and risk of misuse.
To facilitate interfacing with LLMs in the biomedical space, while at the same time safeguarding their functionalities through sensible constraints, we propose a dedicated, open-source framework: BioChatter.
Based on open-source software packages, we synergise the many functionalities that are currently developing around LLMs, such as knowledge integration / retrieval-augmented generation, model chaining, and benchmarking, resulting in an easy-to-use and inclusive framework for application in many use cases of biomedicine.
We focus on robust and user-friendly implementation, including ways to deploy privacy-preserving local open-source LLMs.
We demonstrate use cases via two multi-purpose web apps (https://chat.biocypher.org), and provide documentation, support, and an open community.


## Introduction {.page_break_before}

Despite technological advances, major challenges remain to understand biological and biomedical systems [@gallagher-infinite;@dl-bioscience].
We measure more and more data points with ever-increasing resolution to such a degree that their analysis and interpretation have become the bottleneck for their exploitation [@dl-bioscience].
One reason for this challenge may be the inherent limitation of human knowledge [@doi:10.1016/j.tics.2005.04.010]: Even seasoned domain experts cannot know the implications of every gene, molecule, symptom, or biomarker.
In addition, biological events are context-dependent, for instance with respect to a cell type or specific disease.

Large Language Models (LLMs) of the current generation, on the other hand, can access enormous amounts of knowledge, encoded (incomprehensibly) in their billions of parameters [@doi:10.48550/arxiv.2204.02311;@doi:10.48550/arxiv.2201.08239;@doi:10.48550/arxiv.2303.08774].
Trained correctly, they can recall and combine virtually limitless knowledge from their training set.
ChatGPT has taken the world by storm, and many biomedical researchers already use LLMs in their daily work, for general as well as research tasks [@doi:10.1038/s41586-023-06792-0;@doi:10.1101/2023.04.16.537094;@doi:10.1038/s41587-023-01789-6].
However, the current, predominantly manual, way of interacting with LLMs is virtually non-reproducible, and their behaviour can be erratic.
For instance, they are known to confabulate: they make up facts as they go along, and, to make matters worse, are convinced - and convincing - regarding the truth of their confabulations [@doi:10.1038/s41586-023-05881-4;@doi:10.1038/s41587-023-01789-6].
While current efforts towards Artificial General Intelligence manage to ameliorate some of the shortcomings by ensembling multiple models [@{https://python.langchain.com}] with long-term memory stores [@{https://autogpt.net/}], the current generation of AI does not inspire adequate trust to be applied to biomedical problems without supervision [@doi:10.1038/s41586-023-05881-4].
Additionally, biomedicine demands greater care in data privacy, licensing, and transparency than most other real-world issues [@doi:10.48550/arXiv.2401.05654].

Computational biomedicine involves many tasks that could be assisted by LLMs, such as the interpretation of experimental results, the design of experiments, the evaluation of literature, and the exploration of web resources.
To improve and accelerate these tasks, we have developed BioChatter, a platform for communicating with LLMs specifically tuned to biomedical research (Figure @fig:overview).
The platform guides the human researcher intuitively through the interaction with the model, while counteracting the problematic behaviours of the LLM.
Since the interaction is mainly based on plain text (in any language), it can be used by virtually any researcher.

<!-- Figure 1 -->
![
**The BioChatter composable platform architecture (simplified).**
Many questions arise in daily biomedical research practice, for instance, interpretation of experimental results or the use of a web resource (top left).
BioChatter’s main response circuit (blue) composes a number of specifically engineered prompts and passes them (and a conversation history) to the primary LLM, which generates a response for the user based on all inputs.
This response is simultaneously used to prompt the secondary circuit (orange), which fulfils auxiliary tasks to complement the primary response.
In particular, using search, the secondary circuit queries a database as a prior knowledge repository and compares annotations to the primary response, or uses the knowledge to perform Retrieval-Augmented Generation (RAG).
A knowledge graph such as BioCypher [@biocypher] can similarly serve as knowledge resource or long-term memory extension of the model.
Further, an independent LLM receives the primary response for fact-checking, which can be supplemented with context-specific information by a RAG process.
The platform is composable in most aspects, allowing arbitrary extensions to other, specialised models for additional tasks orchestrated by the primary LLM.
](images/biochatter_overview.png "Overview"){#fig:overview}


## Results

BioChatter (https://github.com/biocypher/biochatter) is a python framework that provides an easy-to-use interface to interact with LLMs and auxiliary technologies via an intuitive API (application programming interface).
This way, its functionality can be integrated into any number of user interfaces, such as web apps, command line interfaces, or Jupyter notebooks.
The framework is designed to be composable, meaning that any of its components can be exchanged with other implementations, for instance, to use a different LLM or knowledge graph (KG).
Functionalities include:

- **basic question answering** with LLMs hosted by providers (such as OpenAI) as well as locally deployed open-source models

- **reproducible prompt engineering** to guide the LLM towards a specific task or behaviour

- **benchmarking** of LLMs, prompts, and other components

- **knowledge graph querying** with automatic integration of any KG created in the BioCypher framework [@biocypher]

- **retrieval-augmented generation** (RAG) using vector database embeddings of user-provided literature

- **model chaining** to orchestrate multiple LLMs and other models in a single conversation using the LangChain framework [@langchain]

- **fact-checking** of LLM responses using a second LLM

In the following, we briefly describe these components, which are demonstrated in our web app (https://chat.biocypher.org).

### Question Answering and LLM Connectivity

The core functionality of BioChatter is to interact with LLMs.
The framework supports both leading proprietary models such as the GPT series from OpenAI as well as open-source models such as LLaMA2 [@doi:10.48550/arXiv.2307.09288] and Mixtral 8x7B [@doi:10.48550/arXiv.2401.04088] via a flexible open-source deployment framework [@{https://github.com/xorbitsai/inference}] (see Methods).
Currently, the most powerful conversational AI platform, ChatGPT (OpenAI), is surrounded by data privacy concerns [@{https://www.reuters.com/technology/european-data-protection-board-discussing-ai-policy-thursday-meeting-2023-04-13/}].
We address this issue in two ways.
Firstly, we provide access to the different OpenAI models through their API, which is subject to different, more stringent data protection than the web interface [@{https://openai.com/policies/terms-of-use}], most importantly by disallowing reuse of user inputs for subsequent model training.
Secondly, we aim to preferentially support open-source LLMs to facilitate more transparency in their application and increase data privacy by being able to run a model locally on dedicated hardware and end-user devices [@doi:10.1038/d41586-023-01295-4].
By building on LangChain [@langchain], we support dozens of LLM providers, such as the Xorbits Inference and Hugging Face APIs [@{https://github.com/xorbitsai/inference}], which can be used to query any of the more than 100 000 open-source models on Hugging Face Hub [@{https://huggingface.co/docs/hub/index}], for instance those on its LLM leaderboard [@{https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard}].
Although OpenAI’s models currently vastly outperform any alternatives in terms of both LLM performance and API convenience, we expect many open-source developments in this area in the future [@biollmbench].
Therefore, we support plug-and-play exchange of models to enhance biomedical AI-readiness, and we implement a bespoke benchmarking framework for the biomedical application of LLMs.

### Prompt Engineering

An essential property of LLMs is their sensitivity to the prompt, i.e., the initial input that guides the model towards a specific task or behaviour.
Prompt engineering is an emerging discipline of practical AI, and as such there are no established best practices [@doi:10.48550/arXiv.2302.11382;@doi:10.48550/arXiv.2312.16171].
Current approaches are mostly trial-and-error-based manual engineering, which is not reproducible and changes with every new model [@biollmbench].
To address this issue, we include a prompt engineering framework in BioChatter that allows the preservation of prompt sets for specific tasks, which can be shared and reused by the community.
In addition, to facilitate the scaling of prompt engineering, we integrate this framework in the benchmarking pipeline, which allows the automated evaluation of prompt sets as new models are published.

### Benchmarking

The increasing generality of LLMs poses challenges for their comprehensive evaluation.
To circumvent this issue, we focus on specific biomedical tasks and datasets, leaving general validation to existing benchmarks.
For advanced assessment, we employ automated validation of the model's responses by a second LLM.
For transparent and reproducible evaluation of LLMs, we implement a benchmarking framework that allows the comparison of models, prompt sets, and all other components of the pipeline.
Built on the generic Pytest framework [@pytest], it allows the automated evaluation of a matrix of all possible combinations of components.
The results are stored and displayed on our website for simple comparison, and the benchmark is updated upon the release of new models and extensions to the datasets.
We create a bespoke biomedical benchmark for multiple reasons: 
Firstly, the biomedical domain has its own tasks and requirements, and creating a bespoke benchmark allows us to be more precise in the evaluation of components [@biollmbench].
Secondly, we aim to create benchmark datasets that are complementary to the existing, general purpose benchmarks and leaderboards for LLMs [@{https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard}].
Thirdly, we aim to prevent leakage of the benchmark data into the training data of the models, which is a known issue in the general purpose benchmarks, also called memorisation or contamination [@doi:10.48550/arXiv.2310.18018].
To achieve this goal, we implemented an encrypted pipeline that contains the benchmark datasets and is only accessible to the workflow that executes the benchmark (see Methods).

**Figure?**

### Knowledge Graphs

Knowledge graphs (KGs) are a powerful tool to represent and query knowledge in a structured manner.
With BioCypher [@biocypher], we have developed a framework to create KGs from biomedical data in a user-friendly manner while also semantically grounding the data in ontologies.
BioChatter is an extension of the BioCypher ecosystem, elevating its user-friendliness further by allowing natural language interactions with the data; any BioCypher KG is automatically compatible with BioChatter.
We use information generated in the build process of BioCypher KGs to tune BioChatter's understanding of the data structures and contents, thereby increasing the efficiency of LLM-based KG querying (see Methods).
In addition, the ability to connect to any BioCypher KG allows the integration of prior knowledge into the LLM's reasoning, which can be used to ground the model's responses in the context of the KG via in-context learning / retrieval-augmented generation (see below).

### Retrieval-Augmented Generation

LLM confabulation is a major issue for biomedical applications, where the consequences of incorrect information can be severe.
One popular way of addressing this issue is to apply "in-context learning," which is also more recently referred to as "retrieval-augmented generation" (RAG) [@doi:10.48550/arxiv.2303.17580].
Briefly, RAG relies on injection of information into the model prompt of a pre-trained model, and as such does not require retraining / fine-tuning; once created, any RAG prompt can be used with any LLM.
While this can be done by processing structured knowledge, for instance from KGs, it is often more efficient to use a semantic search engine to retrieve relevant information from unstructured data sources such as literature.
To this end, we allow the management and integration of vector databases in the BioChatter framework.
The user is able to connect to a vector database, embed an arbitrary number of documents, and then use semantic search to improve the model prompts by adding text fragments relevant to the given question (see Methods).

### Model Chaining and Fact Checking

LLMs cannot only seamlessly interact with human users, but also with other LLMs as well as many other types of models.
They understand API calls and can therefore theoretically orchestrate complex multi-step tasks [@doi:10.48550/arXiv.2305.15334;@doi:10.48550/arXiv.2308.11432].
However, implementation is not trivial and the complex process can lead to unpredictable behaviours.
We aim to improve the stability of model chaining in biomedical applications by developing bespoke approaches for common biomedical tasks, such as interpretation and design of experiments, evaluating literature, and exploring web resources.
While we focus on reusing existing open-source frameworks such as LangChain [@langchain], we also develop bespoke solutions where necessary to provide stability for the given application.
As an example, we implement a fact-checking module that uses a second LLM to evaluate the factual correctness of the primary LLM's responses continuously during the conversation (see Methods).


## Discussion

The fast pace of developments around current-generation LLMs poses a great challenge to society as a whole and the biomedical community in particular [@doi:10.1038/d41586-024-00029-4;@doi:10.1038/d41586-023-03817-6;@doi:10.1038/d41586-023-03803-y].
While the potential of these models is enormous, their application is not straightforward, and their use requires a certain level of expertise.
In addition, biomedical research is often performed in a siloed way due to the complexity of the domain and systemic incentives that work against open science and collaboration [@doi:10.1177/1745691612459058].
Inspired by the productivity of open source libraries such as LangChain [@langchain], we propose an open framework that allows biomedical researchers to focus on the application of LLMs as opposed to engineering challenges.
To keep the framework effective and sustainable, we focus on reusing existing open-source libraries and tools, while adapting the advancements from the wider LLM community to the biomedical domain.
The transparency we emphasise at every step of the framework is essential to a sustainable application of LLMs in biomedical research and beyond [@doi:10.1038/d41586-024-00029-4].

To account for the requirements of biomedical research workflows, we take particular care to guarantee robustness and objective evaluation of LLM behaviour and their performance in interaction with other parts of the framework.
We achieve this goal by implementing a living benchmarking framework that allows the automated evaluation of LLMs, prompts, and other components (https://biochatter.org/benchmark-overview/).
Even the most recent and biomedicine-specific benchmarking efforts are small-scale manual approaches that do not consider the full matrix of possible combinations of components, and many benchmarks are performed by accessing web interfaces of LLMs, which obfuscates important parameters, such as model version and temperature [@biollmbench].
As such, a framework is a necessary step towards the objective and reproducible evaluation of LLMs.
We prevent data leakage from the benchmark datasets into the training data of new models by encryption, which is essential for the sustainability of the benchmark as new models are released.
The living benchmark will be updated with new questions and tasks as they arise in the community.

We facilitate access to LLMs by allowing the use of both proprietary and open-source models, and we provide a flexible deployment framework for the latter.
Proprietary models are currently the most economic solution for accessing state-of-the-art models, and as such primarily suited for users just starting out or lacking the resources to deploy their own models.
In contrast, open-source models are quickly catching up in terms of performance [@biollmbench], and they are essential for the sustainability of the field [@doi:10.1038/d41586-024-00029-4].
We allow self-hosting of open-source models on any scale, from dedicated hardware with GPUs, to local deployment on end-user laptops, to browser-based deployment using web technology.

### Limitations

The current generation of LLMs is not yet ready for unsupervised use in biomedical research.
While we have taken steps to mitigate the risks of using LLMs, such as independent benchmarks, fact-checking, and knowledge graph querying, we cannot guarantee that the models will not produce harmful outputs.
We see current LLMs, particularly in the scope of the BioCypher ecosystem, as helpful tools to assist human researchers, alleviating menial and repetitive tasks and helping with technical aspects such as query languages.
They are not meant to replace human ingenuity and expertise, but to augment it with their complementary strengths.

Depending on generic open-source libraries such as LangChain [@langchain] and Pytest [@pytest] allows us to focus on the biomedical domain but also introduces technical dependencies on these libraries.
While we support those upstream libraries via pull requests, we depend on their maintainers for future updates.
In addition, keeping up with these rapid developments is demanding on developer time, which is only sustainable in a community-driven open-source effort.

### Future directions

Multitask learners that can synthesise, for instance, language, vision, and molecular measurements, are an emerging field of research [@doi:10.48550/arXiv.2306.04529;@doi:10.48550/arXiv.2211.01786;@doi:10.48550/arXiv.2310.09478].
To remain accessible in the face of ever increasing complexity of these models, we will focus on the usability improvements that allow broad adoption in biomedical research. 
Autonomous agents for trivial tasks have already been developed on the basis of LLMs, and we expect this field to mature in the future [@doi:10.48550/arXiv.2308.11432].
As research on agent behaviour progresses, we will integrate these developments into the BioChatter framework to allow the creation of helpful assistants for biomedical research.

All framework developments will be performed in light of the ethical implications of LLMs, and we will continue to support the use of open-source models to increase transparency and data privacy.
While we focus on the biomedical field, the concept of our frameworks can easily be extended to other scientific domains by adjusting domain-specific prompts and data inputs, which are accessible in a composable and user-friendly manner in our frameworks [@biocypher].
Our Python library is developed openly on GitHub (https://github.com/biocypher/biochatter) and can be integrated into any number of user interface solutions.
We develop under the permissive MIT licence and encourage contributions and suggestions from the community with regard to the addition of bioinformatics tool integrations, prompt engineering, benchmarking, and any other feature.

## (Supplementary / Online) Methods

BioChatter is a Python library, supporting Python 3.10-3.12, which we ensure with a continuous integration pipeline on GitHub (https://github.com/biocypher/biochatter).
We provide documentation at https://biocypher.github.io/biochatter, including a tutorial and API reference.
All packages are developed openly and according to modern standards of software development [@doi:10.1038/s41597-020-0486-7]; we use the permissive MIT licence to encourage downstream use and development.
We include a code of conduct and contributor guidelines to offer accessibility and inclusivity to all that are interested in contributing to the framework.

### Applications

To demonstrate basic and advanced use cases of the framework, we provide two web apps, BioChatter Light and BioChatter Next.

BioChatter Light is a web app based on the Streamlit framework (version 1.21.0, https://streamlit.io), which is written in Python and can be deployed locally or on a server (https://github.com/biocypher/biochatter-light).
The ease with which Streamlit allows the creation of interactive web apps in pure Python enables rapid iteration and agile development of new features, with the tradeoff of limited customisation and scalability.
This framework is suited for rapid prototyping of bespoke solutions for specific use cases.
For an up-to-date overview and preview of current functionality of the platform, please visit the [online preview](https://chat.biocypher.org).

BioChatter Next (https://github.com/biocypher/biochatter-next) is a modern web app with server-client architecture, based on the open-source template of ChatGPT-Next-Web (https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web).
It is written combining Typescript and Python and utilises Next.js (v13.4.9) for a sleek frontend and Flask (v3.0.0) as backend.
It demonstrates the use of BioChatter in a modern web app, including full customisation and scalability and localisation in 18 languages.
However, this comes at the cost of increased complexity and development time.
To provide seamless integration of the BioChatter backend into existing frontend solutions, we provide the server implementation at https://github.com/biocypher/biochatter-server and as a Docker image in our Docker Hub organisation (https://hub.docker.com/repository/docker/biocypher/biochatter-server).

We invite all interested researchers to select the framework that best suits their needs, or use the BioChatter server or library in their existing solutions.

### Benchmarking

The benchmarking framework implements a matrix of component combinations using the parameterisation feature of Pytest [@pytest].
This allows the automated evaluation of all possible combinations of components, such as LLMs, prompts, and datasets.
The results are stored in a database and displayed on the website for easy comparison.
The benchmark is updated upon the release of new models and extensions to the datasets.
The individual dimensions of the matrix are:

- **LLMs**: Testing proprietary (OpenAI) and open-source models (commonly using the Xorbits Inference API and HuggingFace models) against the same set of tasks is the primary aim of our benchmarking framework. We facilitate the automation of testing by including a programmatic way of deploying open-source models.

- **prompts**: Since model performance can dramatically rely on the used prompts, a set of prompts for each task with varying degrees of specificity and fixed as well as variable components is used to evaluate this variability.

- **datasets**: We test various tasks using a set of datasets for each task in question-answer-style.

- **data processing**: Some data processing steps can have great impact on the downstream performance of LLMs. 
For instance, we test the conversion of numbers (which LLMs are notoriously bad at handling) to categorical text (e.g., low, medium, high).

- **model quantisations**: We test a set of quantisations for each model (where available) to account for the trade-off between model size and performance.

- **model parameters**: Where suitable, we test a set of parameters for each model, such as "temperature," which determines the reproducibility of model responses.

- **integrations**: We write dedicated tests for specific tasks that require integrations, for instance with knowledge graphs or vector databases.

- **stochasticity**: To account for variability in model responses, we include a parameter to run each test multiple times and generate summary statistics.

- **sentiment and behaviour**: To assess whether the models exhibit the desired behaviour patterns for each of the personas, we let a second LLM evaluate the responses based on a set of criteria, including professionalism and politeness.

The Pytest framework is implemented at https://github.com/biocypher/biochatter/blob/main/benchmark, and more information and results are available at https://biocypher.github.io/biochatter/benchmark.

To prevent leakage of benchmarking data (and subsequent contamination of future LLMs), we implement an encryption routine on the benchmark datasets.
The encryption is performed using a hybrid encryption scheme, where the data are encrypted with a symmetric key, which is in turn encrypted with an asymmetric key.
The datasets are stored in a dedicated encrypted pipeline that is only accessible to the workflow that executes the benchmark.
These processes are implemented at https://github.com/biocypher/llm-test-dataset and accessed from the benchmark procedure in BioChatter.

### Knowledge Graphs

We utilise the close connection between BioChatter and the BioCypher framework [@biocypher] to integrate knowledge graph (KG) queries into the BioChatter API.
In the BioCypher KG creation, we use a configuration file to map KG contents to ontology terms, including information about each of the entities.
For instance, we detail the properties of a node and the source and target classes of an edge.
Additionally, during the KG build process, we enrich this information and save it to a YAML file and, optionally, directly to the KG.
This information is used by BioChatter to tune its understanding of the KG, which allows the LLM to query the KG more efficiently.
By understanding the context of the KG, the exact contents, and the exact spelling of all identifiers and properties, we effectively support the LLM in generating correct queries.
To illustrate the usage of this feature, we provide a demonstration repository at https://github.com/biocypher/pole including a KG build procedure and web app, which can be run using a single Docker Compose command.

### Retrieval-Augmented Generation

While current LLMs possess extensive internal general knowledge, they may not know how to prioritise very specific scientific results, or they may not have had access to some research articles in their training data (e.g., due to their recency or licensing issues).
To bridge this gap, we can provide additional information from relevant publications to the model via the prompt.
However, we frequently cannot add entire publications to the prompt, since the input length of current models still is restricted; we need to isolate the information that is specifically relevant to the question given by the user.
To find this information, we perform a semantic similarity search between the user’s question and the contents of user-provided scientific articles (or other texts).
The most efficient way to do this mapping is by using a vector database [@doi:10.48550/arxiv.2308.07107].

The contextual background information provided by the user (e.g., by uploading a scientific article of prior work related to the experiment to be interpreted) is split into pieces suitable to be digested by the LLM, which are individually embedded by the model.
These embeddings (represented by vectors) are used to store the text fragments in a vector database; the storage as vectors allows fast and efficient retrieval of similar entities via the comparison of individual vectors.
For example, the two sentences “Amyloid beta levels are associated with Alzheimer’s Disease stage.” and “One of the most important clinical markers of AD progression is the amount of deposited A-beta 42.” would be closely associated in a vector database (given the embedding model is of sufficient quality, i.e., similar to GPT-3 or better), while traditional text-based similarity metrics probably would not identify them as highly similar.

By comparing the user’s question to prior knowledge in the vector database, we can extract the relevant pieces of information from the entire background.
Even better, we can first use an LLM to generate an answer to the user's question and then use this answer to query the vector database for relevant information.
Regardless of whether the initial answer is correct, it is likely that the "fake answer" is more semantically similar to the relevant pieces of information than the user's question [@doi:10.48550/arXiv.2308.07107].
Semantic search results (for instance, single sentences directly related to the topic of the question) are then sufficiently small to be added to the prompt.
In this way, the model can learn from additional context without the need for retraining or fine-tuning.
This method is sometimes described as in-context learning [@doi:10.48550/arxiv.2303.17580] or retrieval-augmented generation [@rag].

To provide access to this functionality in BioChatter, we implement classes for the connection to, and management of, vector database systems (in the vectorstore_host.py module), and for performing semantic search on the vector database and injecting the results into the prompt (in the vectorstore.py module).
To demonstrate the use of the API, we add a “Retrieval-Augmented Generation” tab to the preview apps that allows the upload of text documents to be added to a vector database, which then can be queried to add contextual information to the prompt sent to the primary model.
This contextual information is transparently displayed.
Since this functionality requires a connection to a vector database system, we provide connectivity to a Milvus server, including a way to start the server in conjunction with a BioCypher knowledge graph and the BioChatter Light app in one Docker Compose workflow.

### Deployment of Open-Source Models

To facilitate access to open-source models, we adopt a flexible deployment framework based on the Xorbits Inference API [@{https://github.com/xorbitsai/inference}].
We provide Docker images for the automatic deployment of the API and the models.
Xorbits Inference includes a large number of open-source models out of the box, and new models from Hugging Face Hub [@{https://huggingface.co/}] can be added using the intuitive graphical user interface.

In addition, we provide fully browser-based deployment of LLMs using WebAssembly (WASM) and the web-llm library (https://github.com/mlc-ai/web-llm).
We host a local model using web-llm, which is accessed by the BioChatter server within BioChatter Next.
This combination creates a secure conversational environment and minimises the risks associated with data breaches.
Hosting local LLMs using WebLLM allows them to run without an internet connection in a WASM module.
This architecture thus enables complete data security and is limited only by the resources of the host computer.
While the same can be achieved with a local deployment of the Xorbits Inference API, the browser-based deployment is more user-friendly and does not require any additional software.

### Model Chaining

The ability of LLMs to control external software, including other LLMs, opens up a wide range of possibilities for the orchestration of complex tasks.
A simple example is the implementation of a correcting agent, which receives the output of the primary model and checks it for factual correctness.
If the agent detects an error, it can prompt the primary model to correct its output, or forward this correction to the user directly.
Since this relies on the internal knowledge base of the correcting agent, the same caveats apply, as the correcting agent may confabulate as well.
However, since the agent is independent of the primary model (being set up with dedicated prompts), it is less likely to confabulate in the same way.

This approach can be extended to a more complex model chain, where the correcting agent, for example, can query a knowledge graph or a vector database to ground its responses in prior knowledge.
These chains are easy to implement, and some are available out of the box in the LangChain framework [@langchain].
However, they can behave unpredictably, which increases with the number of links in the chain, and as such should be tightly controlled.
They also add to the computational burden of the system, which is particularly relevant for deployments on end-user devices.

## Author Contributions {.page_break_before}

SL conceptualised and developed the platform and wrote the manuscript.
AM implemented the local deployment functionality.
NK implemented benchmarking procedures.
CW architected the BioChatter Next server infrastructure.
QM oversaw the development and deployment of the BioChatter Next server environment.
SF integrated BioChatter continuous integration pipelines and developed both front-end and back-end components for the BioChatter Next server.
JSR supervised the project, revised the manuscript, and acquired funding.
All authors read and approved the final manuscript.

## Acknowledgements

We thank Hanna Schumacher, Daniel Dimitrov, Pau Badia i Mompel, and Aurelien Dugourd for feedback on the original draft of the manuscript and the software.

This work was supported by funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 965193 (SL), award U54-AG075931 (QM) from the National Institutes of Health, award NSF1945971 (QM) from the National Science Foundation, and the Pelotonia Institute of Immuno-Oncology (PIIO).

## Conflict of Interest

JSR reports funding from GSK, Pfizer and Sanofi and fees/honoraria from Travere Therapeutics, Stadapharm, Pfizer, Grunenthal, and Astex Pharmaceuticals.

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>


[@biocypher]: doi:10.1038/s41587-023-01848-y
[@langchain]: https://python.langchain.com
[@pytest]: https://github.com/pytest-dev/pytest
[@biollmbench]: doi:10.1101/2023.12.19.572483
[@dl-bioscience]: doi:10.1038/s41467-022-29268-7
