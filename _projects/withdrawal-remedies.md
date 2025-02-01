---
title: "Studying self-treatment of opioid withdrawal"
collection: projects
category: work
permalink: /project/withdrawal-remedies
excerpt: 'Information extraction using Reddit data.'
date: 2021-01-01
venue:
repourl: 'https://github.com/RTIInternational/withdrawal-remedy-explorer'
appurl: 'https://bit.ly/withdrawal-remedy-explorer'
paperurl: 'https://doi.org/10.2196/33919'
citation:
---

Many people who use opioids self-treat withdrawal symptoms with a range of substances. Little is known about the substances that people use or their effects. 

We developed an information extraction pipeline to identify withdrawal symptom remedies from millions of Reddit posts and comments. The pipeline included named entity recognition, text clustering, and generation of a bipartite substance-effect network. We used the positive pointwise mutual information (PPMI) criterion to identify the most salient remedies. 

This pre-LLM pipeline worked pretty well. If I were to redo this project today, I'd take advantage of newer zero-shot NER algorithms like [GLiNER](https://github.com/urchade/GLiNER) and use LLMs to identify symptom-effect co-occurrence more flexibly. 