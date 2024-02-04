---
title: "Dynamic testing for autonomous vehicles using random Quasi Monte Carlo"
authors:
- Jingwei Ge
- admin
- Cheng Chang
- Yi Zhang
- Danya Yao
- Yonglin Tian
- Li Li
author_notes:
date: "2022-10-01T00:00:00Z"
doi: "10.1109/TIV.2024.3358329"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Vehicles* <br /> (中科院1区期刊; JCR Q1区; 影响因子=8.2)"
publication_short: "IEEE T-ITS"

abstract: The substantial resource usage required to create ample scenarios for testing Autonomous Vehicles (AV) presents a bottleneck in their implementation. At present, research relies on sampling the driving behaviour of Surrounding Vehicles (SV) based on naturalistic datasets in simulation. However, these methods still generate huge amounts of scenarios, making it impossible to synthetically evaluate AV intelligence in a very small number of tests (especially in real-world situations). Simultaneously, the unknown distribution of critical scenarios leads to the problem that more critical scenarios cannot be accurately sampled. In this paper, a novel optimization problem is described and a dynamic scenario sampling method is proposed to cover more critical scenarios with finite samples. First, the sampling space is constructed by extracting the behavioural model parameters of the SVs. Second, multiple rounds of sampling are carried out successively to learn the distribution of critical scenarios, which in turn gradually improves the coverage of the critical scenarios. To do this, in each round, we divide the sampling space into several subspaces using two-step sampling, sample the scenarios using Random Quasi Monte Carlo (RQMC), evaluate the criticality of the subspace, and then use the evaluation results to guide the selection of the sampling space for the next round. The purpose of RQMC is to uniformly sample in the critical subspace rather than Standard Monte Carlo (SMC). Experimental results show that our method can better narrow the gap with the distribution of critical scenarios and discover more critical scenarios when compared to the baseline method.

# Summary. An optional shortened abstract.
summary: In this paper, a novel optimization problem is described and a dynamic scenario sampling method is proposed to cover more critical scenarios with finite samples. 


tags:
- Testing
- Behavioral sciences 
- Monte Carlo methods 
- Sampling methods 
- Vehicle dynamics 
- Autonomous vehicles 
- Automation
featured: false

# links:
# - name: ""
#   url: ""
links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/377439851_Task-Driven_Controllable_Scenario_Generation_Framework_Based_on_AOG
url_pdf: https://www.researchgate.net/profile/Jiawei-Zhang-61
url_code: ''
url_dataset: ''
url_poster: ''
url_project: https://jiaweizhang.netlify.app/project/connected-and-automated-vehicles-simulation-platform/
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: 
  - Connected and Automated Vehicles Simulation Platform

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

 *详细内容请参阅[论文](https://ieeexplore.ieee.org/document/10415067)原文*

<img src=featured.jpg  width=90% />

## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10415067,
  author={Ge, Jingwei and Zhang, Jiawei and Chang, Cheng and Zhang, Yi and Yao, Danya and Tian, Yonglin and Li, Li},
  journal={IEEE Transactions on Intelligent Vehicles}, 
  title={Dynamic Testing for Autonomous Vehicles Using Random Quasi Monte Carlo}, 
  year={2024},
  volume={},
  number={},
  pages={1-13},
  keywords={Testing;Behavioral sciences;Monte Carlo methods;Sampling methods;Vehicle dynamics;Autonomous vehicles;Automation;Intelligence testing;Autonomous vehicles;Multirounds testing;random quasi Monte Carlo},
  doi={10.1109/TIV.2024.3358329}}
```

