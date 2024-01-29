---
title: "Task-driven controllable scenario generation framework based on AOG"
authors:
- Jingwei Ge
- admin
- Cheng Chang
- Yi Zhang
- Danya Yao
- Li Li
author_notes:
date: "2022-10-01T00:00:00Z"
doi: "10.1109/MITS.2023.3319091"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.551)"
publication_short: "IEEE T-ITS"

abstract: Sampling, generation, and evaluation of scenarios are essential steps for intelligent testing of autonomous vehicles. Since uncertainty in driving behavior always leads to different occurrence frequencies of scenarios, we have to sample these scenarios in naturalistic datasets. Furthermore, a specified scenario needs to be further enriched and the driving behavior within it needs to be fully described to carry out generation in simulation systems. However, existing approaches generate scenarios randomly and uncontrollably, which makes them unable to precisely generate the specified scenarios. The driving behavior they describe is also memoryless and inflexible. To address the two issues, we propose a task-driven controllable scenario generation framework that can generate scenarios with the consideration of the driving behavior of Surrounding Vehicles (SVs) in a controllable manner. We first manually assign the driving behavior based on different testing tasks for all the considered vehicles. Then we expand the driving behavior temporally as the continuation and transition of several motion activities and generate the corresponding vehicle trajectories spatially. We adopt And-Or Graph (AOG) to model the transition between these motion activities. In contrast to the common memoryless Markov process, our framework generates driving behavior with continuity and driving memory. Finally, we evaluate our framework by generating lane-changing scenarios.

# Summary. An optional shortened abstract.
summary: This paper propose a task-driven controllable scenario generation framework that can generate scenarios with the consideration of the driving behavior of Surrounding Vehicles (SVs) in a controllable manner.


tags:
- Behavioral sciences 
- Testing 
- Task analysis 
- Scenario generation 
- Autonomous vehicles 
- Uncertainty 
- Trajectory
featured: false

# links:
# - name: ""
#   url: ""
links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/377439851_Task-Driven_Controllable_Scenario_Generation_Framework_Based_on_AOG
url_pdf: https://ieeexplore.ieee.org/abstract/document/10401017
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

 *详细内容请参阅[论文](https://ieeexplore.ieee.org/abstract/document/10401017)原文*

<img src=featured.jpg  width=90% />

## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10401017,
  author={Ge, Jingwei and Zhang, Jiawei and Chang, Cheng and Zhang, Yi and Yao, Danya and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={Task-Driven Controllable Scenario Generation Framework Based on AOG}, 
  year={2024},
  volume={},
  number={},
  pages={1-14},
  keywords={Behavioral sciences;Testing;Task analysis;Scenario generation;Autonomous vehicles;Uncertainty;Trajectory;Scenario generation;AOG;intelligence testing;autonomous vehicles},
  doi={10.1109/TITS.2023.3347535}}
```

