## Supplementary Materials {.page_break_before}

In our Supplementary Notes, we explain the functions of our platform in more detail.
Please note that several of the mentioned features, particularly more advanced ones, are in early developmental stages.

### Prompt Engineering

Recent experience with Large Language Models (LLMs) shows that the clever engineering of model prompts can yield drastic performance increases.
For example, when performing logical inference, simply adding “Let’s think step by step” to the end of a question prompt increased LLM performance from ~20% to ~80% [@doi:10.48550/arxiv.2205.11916].
As such, we highly prioritise the identification and adjustment of prompts tuned exactly to the requirements of the specific task to be performed, respecting “general” rules of interacting with LLMs as well as biomedicine-specific issues.

We designed the backend of ChatGSE to be completely flexible with regard to the application and rearrangement of prompts and prompt templates (which allow the insertion of variables such as the user input question or data).
For templating, we use the corresponding generic functionality provided by LangChain [@{https://python.langchain.com}], while adding our biomedicine-specific layer on top.
We provide general prompts to the primary model, setting it up to be helpful and concise in its responses, and individual prompts for each tool we want the primary model to “understand.”
This includes explanation of the method itself as well as structural information about the data file containing the results.

To make this functionality available to all users, we provide a “Prompt Engineering” tab in the ChatGSE application, which allows the modification (or removal) of existing prompts, as well as the addition of new ones.
We also provide functionality to import and export these prompts in JSON format to facilitate reproducible and shareable biomedical prompt engineering.
To discuss and share examples of useful or ineffective prompts, we encourage all users to join the #biochatter-and-chatgse stream in our freely accessible Zulip channel at https://biocypher.zulipchat.com, or the GitHub discussion thread at https://github.com/biocypher/ChatGSE/discussions/11.

### Correcting Agent

The propensity of LLMs to confabulate untrue facts necessitates control mechanisms and guardrails for their application in research, particularly in high-stakes fields such as biomedicine [@doi:10.1038/s41587-023-01789-6].
Some corrective incentive can be included in the instructions to the primary model, for instance by including a “Criticism” directive such as “Constructively self-criticise your big-picture behaviour constantly.” However, this does not guarantee to prevent confabulations completely, as the same model that confabulates also is responsible for correction.

Thus, we implement a modular combination of primary and corrective model, where the corrective agent – a “second opinion” – is set up with instructions tuned exactly to the task of fact-checking the responses of the primary model (“You are a fact-checker. Please judge the following statement for its factual correctness. ...”).
The performance of the corrective agent can be further increased by using a more powerful model (e.g., moving from gpt-3.5-turbo to gpt-4), by pre-processing the primary model’s response (e.g., splitting the response into single sentences and fact-checking each sentence individually), and comparing the primary model’s statements to prior knowledge stored in a knowledge graph connected to the chat platform.
As model development advances and other parties create models as powerful as OpenAI’s, we foresee it will be useful to combine models from different suppliers to increase diversity between primary and corrective models.
Using ChatGSE’s modular framework, arbitrary numbers of corrective models can be added to the LLM chain.

To allow all users to interact with correcting functionality, we include a dedicated “Corrective Agent” tab for adjusting settings of the corrective model independent of the settings for the primary model.
We also facilitate the testing of corrective agents and their prompts by providing a free-text field for sending false information to the corrective agent.
This is necessary since some models, particularly those from OpenAI, are heavily regulated to not purposely provide false information, even for testing purposes.

The comparative power of the LLM agents can be further increased by connecting to a vector database containing embeddings of the contents of specific user-supplied documents.
For more information, see the following Supplementary Note 3: [In-context Learning].

### Cell Type Annotation

A common repetitive task in bioinformatics is to annotate single-cell datasets with cell type labels.
This task is usually performed by a human expert, who will look at the expression of marker genes and assign a cell type label based on their knowledge of the cell types present in the tissue of interest.
LLMs have been shown to be able to perform this task with high accuracy, and can be used to automate cell type annotation with minimal human input [@doi:10.1101/2023.04.16.537094].

We propose to combine LLM inference on cell types with the storage solutions provided by ChatGSE: using a vector database to store embeddings of cells for a more streamlined workflow, and using a traditional database on the basis of BioCypher [@doi:10.1038/s41587-023-01848-y] to inject prior knowledge into the process, as well as store the intermediate decisions of the model/user.

Using the graphical user interface of ChatGSE, we can provide recommendations of inferred cell types to the human user, such that the ultimate decision about a cell type annotation remains with the domain expert, while the tedious aspects of annotation are reduced significantly.
If the model reaches a threshold of perfect annotation for any cell type (e.g., a >99% success rate in more than 50 cells), the user can decide to trust the model in instances of this cell type and fully automate the annotation in these instances.
Similarly, confidence metrics can be used to trigger user input only at cell type inferences that are not straightforward.

### Causal Inference

More recent models have shown considerable capacity for common sense reasoning, in particular, GPT-4 [@doi:10.48550/arxiv.2303.08774].
There is an unmet need to compare the reasoning outcomes of LLMs to other, more traditional modes of inference, such as the do-calculus [@doi:10.1017/CBO9780511803161], logic models [@doi:10.1038/nrg3885], and semantic reasoning approaches [@doi:10.1145/3357384.3358147].
With ChatGSE, we provide a Python platform for the side-by-side application of reasoning algorithms, in the “Causal Inference” tab.

The ability to connect to flexible databases created by BioCypher enables the representation of the same basic knowledge, but tailored to each individual reasoning mode (for instance, a labelled property graph as input for the logic model, an RDF graph for the semantic reasoner, and a vector database for the LLM).
This increases the ease-of-use as well as the reproducibility of benchmarking the reasoning abilities of different algorithms.

### Literature Reference Database

LLMs are very good feature extractors.
In addition to the correcting agent described in Supplementary Note [Correcting Agent], a “literature agent” can additionally be used to ameliorate the occasionally untruthful statements of the primary model.
Given a response from said model, the literature agent is tasked with extracting references to academic papers from the response (if it contains such), and validating the existence of the claimed reference as well as its attributes (such as title and digital object identifier).
The validation of extracted article authors, titles, and identifiers can be performed by a simple search in a connected database of scientific publications.

### Experimental Design

Experimental design is a crucial step in any biological experiment.
However, it can be a subtle and complex task, requiring a deep understanding of the biological system under study as well as statistical and computational expertise.
LLMs can potentially fill the gaps that exist in most research groups, which traditionally focus on either the biological or the statistical aspects of experimental design.

Similar to the general chat functionality, we provide facilities to upload experimental design plans and ask about their feasibility in the biological or statistical context in an “Experimental Design” tab.
Coupled with a suitable knowledge graph (for instance containing methods literature) and/or a document summarisation of relevant articles, ChatGSE can be a simple and effective tool to consider the design of an experiment from multiple perspectives.

### Podcast my Paper

The recent years have brought significant advances in text-to-speech applications, yielding large accessibility benefits to simple text-based communication and personal assistants.
However, the text of scientific papers is riddled with special characters, references, legends, and entities otherwise hard to interpret by text-to-speech algorithms, such as PCR primer sequences.

To process arbitrary scientific manuscripts into “listenable” text, we create an agent that ingests the paper paragraph-wise and distributes individual sections to an LLM for text cleaning, removing all detracting information, such as reference numbers, web links, figure legends, and statistical information.
The resulting cleaned sections are also lightly summarised to account for consumption by listening, and then fed into a text-to-speech model to generate individual sections (chapters) of the article.
The resulting audio can be played back on any media device.

### Journal Club

In many instances, the evaluation of scientific literature is pursued comparatively.
Whether it is the discussion of which hypothesis is the correct one of two, or which method should be applied to address a specific question, multiple manuscripts need to be integrated to draw conclusions.
We propose to facilitate scientific “discussion” by orchestrating an AI journal club, in which a primary model guides individual models, each responsible for representing one scientific position (e.g., each representing one manuscript).

This way of reasoning has proven effective in the way science is conducted by humans.
By installing dedicated representatives of any position, the argument can be led more effectively, since each participant of the discussion is only responsible for knowing the facts that relate to their own position.
In AI reasoning, problems could arise when one model is responsible for multiple sides of an argument, although for different reasons.
In the case of argument being grounded in a vector database injection process (see Supplementary Note 3: [In-context Learning]), only one model in charge of representing two or more positions (manuscripts) on the matter may become biassed towards a specific position due to multiple issues.
The amount of prompts that can be injected into one model query is limited by the token input length, and sentences from manuscripts that are by chance more similar to the phrase used for the similarity search could become overrepresented in the model’s reasoning.
Using one model per position solves this problem by distributing token limits across multiple models, and by accessing only single manuscripts (or several manuscripts, but from the same “camp”).

The models interact with one another in the way that human discussions are led: the moderator (primary model) gives tasks to the secondary models according to the human researcher’s question, and elicits a response that the adversary needs to address in the next iteration of the discussion.
The discussion, while being autonomous apart from the initial question, can be guided step-by-step by the human researcher.

