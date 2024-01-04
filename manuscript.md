---
title: Molecular Causality in the Age of Foundation Models
keywords:
- systems biology
- biomedicine
- causality
- modelling
- machine learning
- foundation models
lang: en-UK
date-meta: '2024-01-04'
author-meta:
- Sebastian Lobentanzer
- Pablo Rodriguez Mier
- Stefan Bauer
- Julio Saez-Rodriguez
header-includes: |
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta property="og:type" content="article" />
  <meta name="dc.title" content="Molecular Causality in the Age of Foundation Models" />
  <meta name="citation_title" content="Molecular Causality in the Age of Foundation Models" />
  <meta property="og:title" content="Molecular Causality in the Age of Foundation Models" />
  <meta property="twitter:title" content="Molecular Causality in the Age of Foundation Models" />
  <meta name="dc.date" content="2024-01-04" />
  <meta name="citation_publication_date" content="2024-01-04" />
  <meta property="article:published_time" content="2024-01-04" />
  <meta name="dc.modified" content="2024-01-04T15:24:20+00:00" />
  <meta property="article:modified_time" content="2024-01-04T15:24:20+00:00" />
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
  <meta name="citation_author" content="Pablo Rodriguez Mier" />
  <meta name="citation_author_institution" content="Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany" />
  <meta name="citation_author_orcid" content="0000-0002-4938-4418" />
  <meta name="citation_author" content="Stefan Bauer" />
  <meta name="citation_author_institution" content="Helmholtz Zentrum München, -, Neuherberg, Germany" />
  <meta name="citation_author_orcid" content="todo" />
  <meta name="citation_author" content="Julio Saez-Rodriguez" />
  <meta name="citation_author_institution" content="Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany" />
  <meta name="citation_author_orcid" content="0000-0002-8552-8976" />
  <meta name="twitter:creator" content="@saezlab" />
  <link rel="canonical" href="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta property="og:url" content="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta property="twitter:url" content="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta name="citation_fulltext_html_url" content="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta name="citation_pdf_url" content="https://slobentanzer.github.io/causality_perspective_2023/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://slobentanzer.github.io/causality_perspective_2023/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://slobentanzer.github.io/causality_perspective_2023/v/d99702721d457dde1a2b001c63fb60314418fb23/" />
  <meta name="manubot_html_url_versioned" content="https://slobentanzer.github.io/causality_perspective_2023/v/d99702721d457dde1a2b001c63fb60314418fb23/" />
  <meta name="manubot_pdf_url_versioned" content="https://slobentanzer.github.io/causality_perspective_2023/v/d99702721d457dde1a2b001c63fb60314418fb23/manuscript.pdf" />
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
([permalink](https://slobentanzer.github.io/causality_perspective_2023/v/d99702721d457dde1a2b001c63fb60314418fb23/))
was automatically generated
from [slobentanzer/causality_perspective_2023@d997027](https://github.com/slobentanzer/causality_perspective_2023/tree/d99702721d457dde1a2b001c63fb60314418fb23)
on January 4, 2024.
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

+ **Pablo Rodriguez Mier**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-4938-4418](https://orcid.org/0000-0002-4938-4418)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [pablormier](https://github.com/pablormier)
    <br>
  <small>
     Heidelberg University, Faculty of Medicine and Heidelberg University Hospital, Institute for Computational Biomedicine, Heidelberg, Germany
  </small>

+ **Stefan Bauer**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [todo](https://orcid.org/todo)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [tbd](https://github.com/tbd)
    <br>
  <small>
     Helmholtz Zentrum München, -, Neuherberg, Germany
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
✉ — Correspondence possible via [GitHub Issues](https://github.com/slobentanzer/causality_perspective_2023/issues)
or email to
Sebastian Lobentanzer \<sebastian.lobentanzer@gmail.com\>, 
Julio Saez-Rodriguez \<pub.saez@uni-heidelberg.de\>.


:::


## Introduction

Correlation is not causation.
As simple as this widely agreed-upon statement may seem, scientifically defining causality and using it to drive our modern biomedical research is immensely challenging.
Since being described by Aristotle approximately 2500 years ago [@isbn:9781372537233], causal reasoning (CR) remained virtually unchanged until it experienced significant formal and mathematical advancements [@doi:10.1017/CBO9780511803161;@doi:10.1080/01621459.1996.10476902;@isbn:9781400880874] and a resurgence in the field of machine learning (ML) [@causalml] only in recent times.
In parallel, biomedicine has made major leaps in the past century, in particular in the development of high-throughput and large-scale methods.

In the field of systems biology, however, great hopes of causal insights from large-scale omics studies have largely been thwarted by the complexity of molecular mechanisms and the inability of existing methods to distinguish between correlation and causation [@doi:10.1038/nature09534;@doi:10.48550/arXiv.2312.00818].

Randomised clinical trials show that, in a lower-dimensional context, we can reliably identify causal effects.
By controlling “all” relevant covariates in a trial (via the principle of the gold-standard, randomised, double-blind, and placebo-controlled trial) we isolate the causal effect of the controlled variable, i.e., the treatment.
In the language of Pearl’s Do-Calculus [@doi:10.48550/arXiv.1210.4852], we measure the outcome of, for instance, do(“Treat with Vemurafenib”) when conducting a clinical trial on V600E-positive melanoma [@doi:10.1056/NEJMoa1103782].
However, translating this mode of reasoning into the high-dimensional space of modern omics poses enormous challenges.
The dramatically larger parameter space of models at the molecular level leads to problems in the performance of methods and the identifiability of results [@doi:10.1038/s41540-023-00310-8;@doi:10.1371/journal.pone.0027755], as well as in model explainability [@doi:10.48550/arXiv.2309.09901].
With this perspective, we discuss the current connections between CR and molecular systems biology in the context of these challenges.
We will elaborate on three main points:

- biases and what they mean for CR, particularly in the context of biomedical data

- the role of prior knowledge (PK) in CR and how to translate PK into suitable biases

- the role of foundation models in molecular systems biology and their relationship to CR

## Background

### Causal Discovery and Inference

The field of CR distinguishes between causal discovery - the process of building causal hypotheses from data - and causal inference - the process of predicting how a specific situation will turn out given data and the causal relationships known about the system.

Causal discovery is more expensive than inference both computationally and data-wise, because it needs to account for the variability in data generation while isolating generalisable relationships between single measured agents [@doi:10.1146/annurev-statistics-031017-100630].
As a result, most inference mechanisms perform better when including PK at some point in the process, as has been observed in biomedical research
 [@doi:10.1038/nmeth.3773].
For modern systems biology, this means that methods for causal discovery typically require large amounts of experiments. Highly parameterised models such as neural networks increase this requirement even further. As such, many regard causal discovery in molecular biomedicine as a scaling problem [@doi:10.48550/arXiv.2206.10591;@{https://gwern.net/scaling-hypothesis}].

Causal inference, in contrast, focuses on quantifying the causal effects of one variable on another within the framework of already hypothesised causal relationships.
This approach leverages PK about the assumed causal links, which in the causal field are often encoded using directed graphs.
This allows researchers to represent both the causal connections between variables and their directionality, which is required to understand how changes in one variable might lead to changes in another.
For instance, in the case of the RAF-MEK-ERK signalling pathway, a graph would depict RAF activation leading to MEK activation, which in turn leads to ERK activation.
This clear representation of directionality is important for causal inference, as it ensures that analyses focus on the effect of upstream changes on downstream outcomes.
For example, in analysing phosphoproteomic data to assess the impact of inhibiting RAF, a graph-based approach would guide researchers to correctly attribute subsequent changes in ERK to this specific intervention.
Without this causal framework, one might mistakenly interpret correlations as bidirectional influences or overlook confounding factors, leading to incorrect conclusions.
However, inference is also very sensitive to the completeness of the PK that is applied; most biomedical PK is far from complete [@doi:10.15252/msb.202211036].
For instance, the function of more than 95% of all the known phosphorylation events that occur in human cells is currently unknown [@doi:10.1126/scisignal.aau8645; @doi:10.1038/s41587-019-0344-3].
In contrast to causal discovery, scaling therefore plays a smaller role in causal inference; here, the main problems are incompleteness and identifying the “right” biases to apply.

### The Ladder of Causality

Orthogonally to the distinction between causal discovery and inference, we can also distinguish between different levels of causality.
Pearl’s ladder of causality roughly distinguishes three types of CR in increasing order of power: observation, intervention, and counterfactuals [@isbn:9780465097609].
While the inferences we wish to make in biomedical research are often of the counterfactual type (e.g., “would RAF inhibition lead to decrease in ERK activation if the media contained Epidermal Growth Factors?”), the data we have available is typically observational (e.g., “the levels of RAF and MEK activity are correlated”) and sometimes interventional (e.g., “targeting RAF with CRISPR leads to a decrease in ERK activity”).
To generate interventional or even counterfactual inferences from observational data is a major challenge, if not impossible, depending on the characteristics of the system under study [@doi:10.1214/09-SS057].

There are approaches to delineate interventional inference from observational data, such as the ‘natural experiments’ framework [@doi:10.1080/01621459.1996.10476902;@isbn:9781400880874].
However, these approaches are by their nature even more data-hungry than when using interventional data, as they necessarily discard information that is not relevant to the intervention.
Therefore, in biomedical research, there has been a push towards generating large-scale interventional data, for instance through the use of CRISPR/Cas9 screens with single-cell resolution [@doi:10.1016/j.cell.2016.11.038].
Current developments of CR in the biomedical field thus mostly focus on these types of data.

### Deduction and Induction

Lastly, in CR, we can also distinguish between deductive and inductive reasoning.
Deductive reasoning is the process of deriving a conclusion from a set of fixed and known premises.
“All men are mortal, Socrates is a man, therefore Socrates is mortal” is a classic example of deductive reasoning.
In biomedical research, this is typically the process of deriving a conclusion from a set of PK.
For instance, having PK of the linear activation cascade EGFR->RAS->RAF->MEK->ERK->Growth, and that Vemurafenib will inhibit RAF activity, allows us to deduce that giving Vemurafenib will inhibit growth of cancer cells [@doi:10.1056/NEJMoa1103782].

Inductive reasoning, on the other hand, involves making generalisations from specific observations.
Testing the hypothesis above, we apply Vemurafenib in a clinical trial of V600E-positive melanoma and find that it is clinically efficacious [@doi:10.1056/NEJMoa1103782].
We could now infer (via induction) that Vemurafenib may be an effective remedy in other V600E-positive cancers as well, or, further, that inhibiting this cascade may be a general mechanism of action of anti-cancer agents in cancers that display MAPK pathway overactivation [@doi:10.1038/nrd3847].
In the molecular realm, we could further infer that the inhibition of other components of the cascade, such as EGFR or MEK, may also be promising target leads [@doi:10.3390/ijms20061483].

The main difference between deduction and induction is that the former is logically complete - i.e., if the premises are true and the argument is valid, the conclusion must also be true.
However, deduction is also more limited in scope than induction.
In biomedical research, we often have to rely on inductive reasoning because we cannot feasibly test all hypotheses in a deductive manner.
In consequence, the *inductive biases* we introduce into our models (i.e., those mechanisms in the model that help with inductive reasoning) are a pivotal part of performing CR in biomedical research.


## Bias

### Meaning and examples of biases

Biases, generally, are systematic prejudices of a model towards certain outcomes.
Humans make frequent use of biases to function in a complex world with limited cognitive resources [@doi:10.1037/0033-295X.111.1.3].
In fact, we often deduce causality from observation (i.e., we “jump to conclusions”), which is indicative of a strong inductive bias [@doi:10.1126/science.1192788].
A good *heuristic* is the application of a suitable bias to a problem, such that the solution can be considered acceptable despite limited resources.

In machine learning (ML), we can distinguish between useful and harmful biases.
Harmful biases are common issues in the technical process of training models; they include, for instance, sampling bias, selection bias, confirmation bias, overfitting, and underfitting [@doi:10.48550/arXiv.1908.09635].
While addressing harmful biases is a crucial part of ML, we will not discuss them further in this perspective.

Useful biases, on the other hand, are biases that are introduced into a model to improve its performance.
Since most models developed in biomedical research and the broader ML community are inductive models, one of the most discussed useful biases is *inductive bias*.
For instance, PK on protein interactions can impact inference on activation cascades; only upstream proteins can activate downstream proteins, not vice versa.

### Why do we need biases?

The human mind will be the gold standard for reasoning for the foreseeable future.
However, human reasoning is limited by our sensory and mnemonic capacity; we cannot reason about high-dimensional data since we can neither perceive it nor keep it in memory.
Machine learning seems like the ideal solution, but the "No Free Lunch" theorems present a fundamental challenge: no single learning algorithm may be universally superior across all problem domains [@no-free-lunch;@doi:10.1613/jair.731;@doi:10.48550/arXiv.2304.05366].
Although they have recently been challenged [@doi:10.48550/arXiv.2304.05366], these theorems highlight the inherent difficulty in designing algorithms that generalise well from specific training data to new, unseen data.
Inductive biases guide algorithms in making educated guesses about unseen data, thereby improving their generalisation capabilities [@doi:10.1098/rspa.2021.0068].

This need for inductive biases is particularly apparent in the realm of biomedicine [@doi:10.1038/s41467-022-29268-7].
Biomedical research operates within a framework constrained by limited and often high-dimensional data, stemming from the high costs of experiments, the scarcity of samples, and the inherent complexity of biological systems.
Coupled with the natural variability of biological measurements, these factors result in a low signal-to-noise ratio, making it challenging to discern meaningful patterns.
Inductive biases direct the learning process towards more relevant solutions by incorporating assumptions that enable more effective learning and interpretation, ensuring that models are not just statistically sound but also biologically meaningful.

Some central questions then arise: 

- How explicit should we be in introducing biases, i.e., should the model determine its own biases, or do we force them on the model?

- How do we choose the right biases to introduce?

- How do we evaluate the biases we introduce?


## Bias from prior knowledge

The first question alone is highly debated in the wider field of ML.
The frequently quoted “Bitter Lesson” posits that we should refrain from inducing all but the most basic biases in our models, and that we should not view metrics as the ultimate measure of performance, but rather whether the model gets us closer to some truth [@{http://www.incompleteideas.net/IncIdeas/BitterLesson.html}].
However, it has been argued that many improvements that led to the models of today, such as convolution or attention, disprove this theory [@doi:10.48550/arXiv.1706.03762], and that the intrinsic complexity of real-world systems does not obviate, but rather necessitate, the integration of human insight into our learning frameworks [@{https://rodneybrooks.com/a-better-lesson/}; @{https://threadreaderapp.com/thread/1106534178676506624.html}].

In systems biology, specifically, there is much interest in finding models with suitable biases to deal with constraints specific to the field, such as data availability and the completeness of PK [@doi:10.48550/arxiv.1811.12359;@doi:10.1109/JPROC.2021.3058954;@doi:10.48550/arxiv.2106.12430;@doi:10.48550/arXiv.2312.00818;@doi:10.1098/rspa.2021.0068].
Considering these constraints, the question is not whether to include PK in our reasoning, but which knowledge, when, and how [@{https://threadreaderapp.com/thread/1106534178676506624.html}].

### Prior knowledge

PK refers to information or data that is available to inform a learning process, enhancing the performance of the trained models and their ability to generalise.
It can be used to inform the inductive biases of a model, either explicitly through the design choices and assumptions embedded into the models, or implicitly through the data and methods used in training.
For this to be possible, biomedical entities and relationships must be clearly defined and represented unambiguously.
Additionally, the diversity in our tasks and knowledge sources requires a flexible representation.
Knowledge representation frameworks can aid in this process [@doi:10.1038/s41587-023-01848-y].

In the biomedical field, there is a rich tradition of documenting biological knowledge at various levels of detail and focusing on different aspects of biology.
Detailed mechanistic models provide mathematical descriptions of the dynamic interactions at a molecular or cellular level.
Genome-scale networks, including metabolic and gene regulatory networks, offer comprehensive views of metabolic processes and gene interactions [@doi:10.1038/nrg3885].
Protein-protein interaction databases recapitulate either causal or non-causal interactions between proteins [@doi:10.1038/nrg3885].

### Modelling on prior knowledge

The integration of PK into models is a non-trivial but essential process for moving from correlation to causation.
PK can be used to derive inductive biases either *explicitly* or *implicitly*.

The explicit case typically involves a mathematical framework where a set of assumptions is explicitly stated and integrated into the model.
Ordinary Differential Equation (ODE) models [@doi:10.1007/978-3-642-38874-3_2], logic-based models [@doi:10.1021/bi902202q], rule-based models [@doi:10.1002/wsbm.1245], constraint-based models [@doi:10.1038/nrg3643], and Structural Causal Models (SCMs) [@doi:10.48550/arXiv.2310.14935]: all explicitly incorporate different types of PK, can be fitted to data, and then be used to answer different types of causal questions.
Their advantage is high efficiency in the face of scarce data, but they are highly reliant on the quality and comprehensiveness of the underlying PK [@doi:10.1103/PhysRevResearch.5.043252].

In contrast, implicit integration of PK in models involves learning useful representations directly from the data, without the explicit inclusion of biological assumptions or causal knowledge.
These can be simple or elaborate.
Simple implicit biases include regularisation techniques that help models generalise by preventing overfitting [@doi:10.1111/j.2517-6161.1996.tb02080.x], or decisions about the types of prior distributions in bayesian models [@doi:10.1038/s41467-017-02554-5].
More elaborate are neural networks which employ specific architectural designs, such as Convolutional Neural Networks (CNNs) [@doi:10.1162/neco.1989.1.4.541​], Recurrent Neural Networks (RNNs) [@doi:10.1162/neco.1997.9.8.1735], or Transformers [@doi:10.48550/arXiv.1706.03762].
Their advantages and disadvantages are inverse to those of explicit models [@doi:10.1103/PhysRevResearch.5.043252].

As a result, choosing the best way to derive inductive biases from PK is not straightforward.
Models that explicitly incorporate PK are more interpretable and can generalise effectively even when data is scarce.
However, they are constrained by the accuracy of the existing knowledge and often struggle to scale to larger datasets [@doi:10.48550/arXiv.2001.08361;@doi:10.48550/arXiv.2202.05808].
Models with implicit biases, on the other hand, particularly those typically found in deep learning architectures, excel at learning from large, high-dimensional datasets and offer flexibility across diverse domains.
Yet, they suffer from limited interpretability, are prone to overfitting, and typically do not generalise well to scenarios not encountered during training, such as predicting the effects of new drugs or drug combinations, largely due to their lack of causal knowledge.

Hybrid models make a tradeoff between those extremes, which is why they have been found to be useful in systems biology, where data are currently scarce [@doi:10.1038/s41592-021-01283-4;@doi:10.1038/s41467-022-30684-y;@doi:10.1038/s41467-023-40380-0;@doi:10.1038/s41587-023-01905-6;@doi:10.1186/s13059-020-02100-5;@doi:10.1038/s41556-022-01072-x;@doi:10.1016/j.cels.2020.11.013].
While their implementation details differ, they often employ two learners side-by-side, one of which is driven by explicit biases from PK, while the other learns from data.
Frequently, these learners are also coupled in an end-to-end learning process, i.e., they “learn together.” This mode of learning aims to benefit from the “bias-free” nature of neural networks while simultaneously improving model performance in the face of scarce data via the added explicit bias.



## Causality in foundation models

There has been an enormous spike of interest in attention-based neural network models, in large part due to the success of Large Language Models (LLMs).
While the high performance of LLMs is based on myriad architectural improvements, the introduction of attention as an architectural bias has been a major contributor to their success [@doi:10.48550/arXiv.1706.03762].
This has led to the development of attention-based molecular models (most commonly for gene expression), which can also be considered “GPT” models: Generative Pre-trained Transformers [@doi:10.1038/s41592-021-01252-x;@doi:10.1038/s41586-023-06139-9;@doi:10.1101/2023.04.30.538439].
Attention as a learning mechanism enables the integration of non-local information in a flexible manner.
In a molecular model that reasons about gene expression, such as Geneformer, attention allows the integration of distant regulatory elements [@doi:10.1038/s41586-023-06139-9].
Notably, this mechanism comes with a computational cost that increases exponentially with respect to the length of the input sequence [@doi:10.48550/arXiv.2310.05869].

The generalist capabilities of LLMs have led to the designation of “foundation models” [@{https://crfm.stanford.edu/}].
Foundation models are models that achieve high performance by training a generic architecture on extremely large amounts of data in an unsupervised manner.
They can be fine-tuned for more specific tasks, because they are thought to derive generalisable representations and mechanisms by training on an amount of data large enough to learn the complexity of real-world systems.
However, recent molecular foundation model benchmarks highlight clear discrepancies between the “foundational” aspirations of the pre-trained models and the real-world evaluation of their performance [@doi:10.1101/2023.10.16.561085;@doi:10.1101/2023.10.19.563100].
Briefly, the benchmarks found that, on single cell classification tasks, the proposed foundation models did not outperform simple baselines consistently.
State-of-the-art methods such as scVI [@doi:10.1038/s41592-018-0229-2] and even the mere selection of highly variable genes was often statistically indistinguishable from the highly parameterised methods, and sometimes even yielded better classification outcomes.
However, these are early models, and it could still be argued that, in line with the scaling hypothesis, models will improve via a combination of the right architecture with sufficient amounts of data.

Indeed, molecular foundation models lag behind in size: while current-generation LLMs have around 100 billion parameters or more and are trained on enormous text corpuses (hundreds of billions to trillions of tokens), molecular foundation models have tens of millions of parameters (scGPT: 53M, Geneformer: 10M) and are trained on corpuses of tens of millions of cells, which (optimistically) yields hundreds of billions of individual data points.
Thus, LLMs are currently about 2000 times larger than molecular foundation models, while arguably also dealing with a less complicated system.
The question whether scaling will lead to the emergence of “foundational behaviour” in molecular models is still a matter of much debate.

### Attention - and large amounts of data - is all you need?

Given enough data to train on - and ample funds for compute - is attention “all you need” to induce reliable biases in your model?
While there are doubts regarding the reasoning capabilities of LLMs, GPT arguably “understands” language very well already, to the point where it can flawlessly communicate and synthesise information [@doi:10.1038/d41586-023-02361-7].
This is what the term “foundation model” implies: the model has derived a generalisable representation of language, a tool that can be fine-tuned for a variety of language-related tasks.
This behaviour is not possible without assuming some form of causality, even if it is not explicitly encoded in the model [@doi:10.48550/arXiv.2206.10591].

In this light, what are the reasons to be sceptical about the capacity of molecular foundation models to understand the “grammar” of the cell?

**Explainability**: For one, large transformer models are not explainable due to their large number of parameters and non-linearities.
As such, there is no way to scrutinise their reasoning beyond the output they produce.
What seems simple in the case of language models - the famous Turing test can be performed by any human with a basic understanding of language - is exceedingly difficult in the molecular space, where many causal relationships are still unknown [@doi:10.1038/d41586-023-02361-7].
Yet the only way to scrutinise and subsequently improve the reasoning capabilities of a model is precisely this explicit validation of its predictions in an interpretable setting.

While the creation of explicit molecular models (e.g., logic, structural causal, or ODE-based models) and the self-supervised training of molecular foundation models are methodically very different, both can provide a hypothesis on causal structure that can be formulated as a network.
Theodoris et al. explore the attention layers of their Geneformer foundation model to explain the model’s reasoning [@doi:10.1038/s41586-023-06139-9].
While some layers show clear patterns of attention, such as attending to highly connected or highly expressed genes, other layers are not as readily interpretable, much less so than explicit molecular models.

**Benchmarking**: Whether these complex layers reflect the true complexity of the underlying biology or are rather evidence for overfitting to the training data is not clear.
One argument in favour of overfitting is the poor generalisation of the model in independent benchmarks [@doi:10.1101/2023.10.16.561085; @doi:10.1101/2023.10.19.563100].
To determine whether molecular foundation models indeed capture generalisable causal representations of biology, dedicated benchmarks are needed.

**Causal bias**: The GPT-3 architecture that led to the recent breakthrough in LLM capabilities employs “causal self-attention,” describing an implicit architectural bias that prevents the model from “looking into the future”: for predicting the next token, only the previous tokens in the sentence can be used [@doi:10.48550/arXiv.2310.05869].
This leverages the implicit causality present in language, which incidentally is similar to one of the earliest formal descriptions of causality, that “the effect has regularly followed the cause in the past” [@isbn:9780199211586].
Compared to language, the data that form the input of molecular foundation models do not have an implicit form of causality.
The individual cells are in general not on a known temporal trajectory, and the genes that are masked as part of the training objective are masked at random, not because they are downstream (in some form) of the genes used for prediction.
This fundamental difference between language and molecular models has so far not been explored theoretically or empirically.

### Causal latent spaces

Due to the fundamental limitation of human perception, dimensionality reduction is a popular workflow for data interpretation, typically via methods such as PCA, t-SNE, or UMAP [@doi:10.4236/jdaip.2021.93013].
The hope is that exploration and explanation in the lower-dimensional embedding space may be less challenging than in the original data, which assumes that the most important aspects of variability in the original data are captured in the reduced dimensions.
However, without explicit supervision, which is rare in typical biomedical datasets, the resulting latent spaces are rarely interpretable, and do not lend themselves to causal interpretation.
In addition, they often suffer from biases that result from technical rather than biological factors [@doi:10.1371/journal.pcbi.1011288].
In consequence, biological insight during the exploration of these latent spaces is often challenging due to the dominance of biases over the biological generative mechanism.

Performing causal inference in latent spaces could potentially solve some of these issues.
“Moving through the latent space” reduces the number of variables that change upon intervention, making exploration simpler in theory.
In practice, however, ease and sensibility of exploration depend completely on whether the inductive biases in the embedding process capture the underlying biology.
In addition, latent spaces have no trivial connection to the real-world measurements they are based on.
Each model instance generates its own, independent latent space; in consequence, the exploration of latent spaces is challenging and time-consuming.

Even if a given latent space can be explored, there is often no guarantee that interpolation between sensible latent representations also leads to sensible results.
As an example, consider a prevailing issue of visual generative models in drawing human hands: images of hands typically involve mangled anatomy and an incorrect number of digits [@{https://www.newyorker.com/culture/rabbit-holes/the-uncanny-failures-of-ai-generated-hands}].
Even though there is a section in the latent space that represents hands, this does not represent the concept of a hand, but rather is guided by learning on many diverse pictures of hands.
A section of this latent space may represent only a finger, and carry some information that next to a finger there usually is another finger.
However, when generating the image, there is no mechanism to keep track of how many digits to add to any generated hand, leading to wrong anatomy.
Similarly, when exploring the latent space of a model of molecular signalling, there may be no guarantees that the model respects the concept of a given pathway when generating the signalling molecules involved.

If mastered, exploring and performing interventions in latent spaces promises many benefits: better generalisation and improved sample efficiency [@doi:10.1109/JPROC.2021.3058954], predicting the outcomes of interventions not observed at training time [@doi:10.48550/arXiv.2310.04295], or insights into the effect of different inductive biases in the model [@doi:10.48550/arXiv.2107.00793].
However, to achieve this, gaining a better understanding of properties of the learned embeddings and variables is essential, for instance by performing “imagined interventions” in the latent space [@doi:10.48550/arXiv.2106.16091] or by using model uncertainty for guiding the optimisation process in the latent space [@doi:10.48550/arXiv.2107.00096].
Of note, many of the proposed solutions for more explainable latent spaces depend on architectures that may scale significantly worse than transformers [@doi:10.48550/arXiv.2001.08361;@doi:10.48550/arXiv.2202.05808].


## Discussion / Conclusion

### Dichotomy of Scaling (data-driven) and Bias Injection (knowledge-driven)

The debate between adopting scaling strategies versus the injection of biases from PK highlights a fundamental tension in modern biomedical research.
The "Bitter Lesson" suggests a preference for general-purpose learning algorithms that scale with computational resources, implicitly learning biases from data.
Conversely, explicitly injecting biases from PK can lead to more specialised and efficient models that can generalise using relatively little training data, but may not scale.
Hybrid models currently represent a promising middle ground, combining the scalability of generalist models with the efficiency and specificity provided by tailored biases.
Researchers often rely on intuition to determine which biases to inject, understanding that while no single model may universally excel (reflecting the "No Free Lunch" theorem), the blend of generalisation through scaling and specialisation through bias injection might provide a robust framework for tackling complex biomedical challenges.
In addition, complex models often pose computational challenges; many models are limited to network sizes of <10 nodes, and feedback loops are often excluded.

### Theoretical Foundations: Interventions and Inductive Biases

Theoretical work emphasises the need for interventions in causal discovery but does not yet address the influence of inductive biases [@doi:10.48550/arXiv.1207.1389].
The number of required interventions might be reduced significantly when complemented with high-quality observational data and appropriate biases, as suggested by neural causal models [@doi:10.48550/arXiv.1910.01075].
However, the precise nature of these biases and their impact remains understudied theoretically as well as empirically.
The comparative effectiveness and theoretical underpinnings of explicit models versus implicit models are particularly understudied.
Foundation models have embraced causal masking as a step towards integrating causality, but this alone may be insufficient.
Empirical studies and more robust theories are needed to understand these dynamics, including the potential existence and validation of causal latent spaces.

### Data Types: Observational vs. Interventional

The choice between training on observational versus interventional data (or a mixture of both) is critical in the development of models.
While large-scale data collection is vital, the type of data collected can significantly influence model performance and the ability to generalise and make accurate causal inferences.
Observational data are more readily available but may lead to confounded or biassed insights.
Interventional data, while more challenging to obtain, provide clearer causal pathways and can greatly enhance the model's understanding of underlying biological processes.
A balanced approach, possibly incorporating both data types, might provide a more nuanced understanding and improve model robustness and interpretability.

### Foundation Models: Architectural Biases and the No Free Lunch Theorems

Foundation models challenge the "No Free Lunch" theorems by suggesting that certain architectural biases, learned from vast amounts of data, can yield generalisable and high-performing models.
These biases, and how to transfer them from LLMs to systems biology, necessitate careful evaluation.
As the biomedical field looks to these models for answers, it becomes crucial to develop frameworks that facilitate rapid development and exploration of ideas [@doi:10.48550/arXiv.2304.05366;@doi:10.1038/s41587-023-01848-y;@doi:10.48550/arXiv.2210.17283].

### Systems Biology and Implicit Causality

Systems biology has always engaged with causal reasoning, aiming to understand the complex mechanisms underlying biological systems.
New methods and models offer the potential to scale this understanding to larger, more complex systems.
The impact of these methods will depend on the successful integration of appropriate algorithms, biases, and data types.
The field stands at a crossroads, determining whether the future of biological modeling will be dominated by the generation of vast datasets for generalist models or by more nuanced, bias-inclusive architectures.
This decision will significantly influence the direction and effectiveness of future research in systems biology.

### Combining Algorithms and Biases with Data Types for Impactful Biological Modeling

While the allure of generalist models trained on extensive datasets is strong, the unique challenges of biomedical research may necessitate a more tailored approach.
Including explicit favourable biases, informed by deep domain knowledge and specific data types (observational or interventional), could lead to breakthroughs in understanding complex biological systems.
The field must explore these possibilities, balancing the drive for large-scale data with the need for precision and specificity, to realise the full potential of modern systems biology.


## Glossary?

## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>

