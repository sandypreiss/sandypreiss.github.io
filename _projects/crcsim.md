---
title: "CRCsim"
collection: projects
category: work
permalink: /project/crcsim
excerpt: 'Microsimulation of colorectal cancer screening cost effectiveness.'
date: 2020-01-01
venue:
repourl: 'https://github.com/RTIInternational/crcsim'
appurl:
paperurl: 'https://doi.org/10.1002/cncr.70436' 
citation:
---

I ported this colorectal cancer microsimulation model from proprietary software (AnyLogic) to Python. I also architected AWS tooling to run large simulation experiments. We've used it to study topics like:

- What long-term impacts are expected from an intervention to increase cancer screening rates?
- What about long-term impacts from a policy change that decreases health insurance coverage?
- What is the relative cost effectiveness of various screening recommendations and tests?

Most recently, I ported the post-simulation analysis step from Pandas to Polars, netting a 38x speedup. This made frequent model recalibration feasible for the first time, so I also developed a calibration framework using Optuna. We can now fully calibrate the model in minutes, which opens up a new range of experiments, such as demographic comparisons where a versio of the model is calibrated to each demographic's colorectal cancer incidence and survival rates.
...