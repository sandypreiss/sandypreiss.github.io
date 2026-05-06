---
title: "Differentially private deep learning for survey autocoders"
collection: projects
category: work
permalink: /project/swag-ppm
excerpt: 'Novel methods to enable public release of models trained on private data.'
date: 2026-01-01
venue:
repourl:
appurl:
paperurl: 'https://arxiv.org/abs/2503.21528'
citation:
---

For the Bureau of Labor Statistics (BLS), my team is developing methods to enable releasing machine learning [models](https://www.bls.gov/iif/automated-coding.htm) trained on sensitive data with formal privacy guarantees. We’re addressing a problem agencies are increasingly facing: models—not just data products—are becoming public-facing assets, and they can leak training data through membership inference and related attacks.

We developed a novel method called SWAG‑PPM, a Bayesian approach to differentially private deep learning that concentrates privacy protection on high‑risk records. This contrasts with common methods like differentially private stochastic gradient descent [DP-SGD](https://arxiv.org/abs/1607.00133), which apply uniform noise. The effect is that privacy distortion is confined mostly to high‑risk tail records, while modal regions—where most utility comes from—remain largely intact.

We're currently piloting SWAG-PPM with a model used to classify open-text responses on the Survey of Occupational Injuries and Illnesses. To enable this, I used Claude Code to refactor an experimental codebase to a production-ready system. This makes it easy for us to run training experiments at scale with only a few tweaks to config files.