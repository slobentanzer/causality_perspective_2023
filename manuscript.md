---
title: Causality - Perspective
keywords:
- biomedicine
- causality
- modelling
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
  <meta name="dc.title" content="Causality - Perspective" />
  <meta name="citation_title" content="Causality - Perspective" />
  <meta property="og:title" content="Causality - Perspective" />
  <meta property="twitter:title" content="Causality - Perspective" />
  <meta name="dc.date" content="2023-10-27" />
  <meta name="citation_publication_date" content="2023-10-27" />
  <meta property="article:published_time" content="2023-10-27" />
  <meta name="dc.modified" content="2023-10-27T13:50:15+00:00" />
  <meta property="article:modified_time" content="2023-10-27T13:50:15+00:00" />
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
  <link rel="canonical" href="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta property="og:url" content="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta property="twitter:url" content="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta name="citation_fulltext_html_url" content="https://slobentanzer.github.io/causality_perspective_2023/" />
  <meta name="citation_pdf_url" content="https://slobentanzer.github.io/causality_perspective_2023/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://slobentanzer.github.io/causality_perspective_2023/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://slobentanzer.github.io/causality_perspective_2023/v/ff3b8cc09436e0ff099c82b8dd2e808310680dee/" />
  <meta name="manubot_html_url_versioned" content="https://slobentanzer.github.io/causality_perspective_2023/v/ff3b8cc09436e0ff099c82b8dd2e808310680dee/" />
  <meta name="manubot_pdf_url_versioned" content="https://slobentanzer.github.io/causality_perspective_2023/v/ff3b8cc09436e0ff099c82b8dd2e808310680dee/manuscript.pdf" />
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
([permalink](https://slobentanzer.github.io/causality_perspective_2023/v/ff3b8cc09436e0ff099c82b8dd2e808310680dee/))
was automatically generated
from [slobentanzer/causality_perspective_2023@ff3b8cc](https://github.com/slobentanzer/causality_perspective_2023/tree/ff3b8cc09436e0ff099c82b8dd2e808310680dee)
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
✉ — Correspondence possible via [GitHub Issues](https://github.com/slobentanzer/causality_perspective_2023/issues)

:::


## Abstract {.page_break_before}




## Introduction

Correlation is not causation.
As simple as this widely agreed-upon statement may seem, scientifically defining causality and using it to drive our modern biomedical research is immensely challenging.
Since being described by Aristotle approximately 2500 years ago, causal reasoning (CR) remained virtually unchanged [@isbn:9781330267608] until  significant formal and mathematical advancements in the last decades [@doi:10.1017/CBO9780511803161, @doi:10.1080/01621459.1996.10476902, @isbn:9781400880874].
In parallel, biomedicine has made major leaps in the past century, in particular in the development of high-throughput and large-scale methods.

Randomised clinical trials show that, in a lower-dimensional context, we can achieve the high levels of confidence needed to satisfy the ethical requirements of modern medicine.
However, translating this mode of reasoning into the high-dimensional space of modern omics is met with enormous challenges.
The dramatically increased parameter space of models at the molecular level leads to problems in the performance of methods and the identifiability of results, as well as in model explainability.

With this perspective, we want to encourage and guide the use of CR to inform biomedical problems and vice versa.
We will elaborate on three main points:

- biases and what they mean for CR, particularly in the context of biomedical data

- the role of prior knowledge in CR and how to translate prior knowledge into suitable biases

- the role of foundation models in molecular systems biology and their relationship to CR

## Bias

### Meaning and examples of biases

### Why do we need biases?



## Bias from prior knowledge

### Prior knowledge

OmniPath/BioCypher

Ontologies

### Modelling on prior knowledge

Statistical, causal, and mechanistic models

Why modelling needs biases and how to introduce them

## Causality in foundation models

Current interest in transformers

Recent foundation model benchmarks

Is attention (and large amounts of data) “all you need” to induce reliable biases in your model? (GPT “understands” language well) [@doi:10.1038/d41586-023-02361-7]

What is the mathematical relationship between explicit (e.g. ODE) and implicit (transformers) models?

Latent encodings of explicit prior knowledge (GEARS)


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>

