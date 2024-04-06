---
title: "Adversarial Generation of Safety-Critical Lane-Change Scenarios for Autonomous Vehicles"
authors:
- Zimin He
- admin
- Danya Yao
- Yi Zhang
- Huaxin Pei
author_notes:
date: "2022-10-09T00:00:00Z"
doi: "10.1109/ITSC57777.2023.10422684"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-09T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*2023 IEEE 26th International Conference on Intelligent Transportation Systems (ITSC)*"
publication_short: "IEEE ITSC"

abstract: traffic, and testing in safety-critical scenarios is essential for identifying scenarios that autonomous vehicles cannot handle. Given the rarity of safety-critical scenarios, it is necessary to investigate how to systematically generate these scenarios. In this paper, we propose an adversarial method to efficiently generate safety-critical scenarios through deep reinforcement learning. We first formulate the typical lane-change scenarios based on the Markov Decision Process and then train the background vehicles to aggressively interfere with the autonomous vehicle under test and create some risky situations. We also propose a reasonableness reward to avoid the extreme adversarial behavior of the background vehicles, making the scenarios reasonable and informative for the autonomous vehicle testing. Simulation results show that the generated scenarios are more critical in terms of safety than those in the naturalistic environment, significantly degrading the performance of the vehicle under test and providing a basis for improving the model.

# Summary. An optional shortened abstract.
summary: 一种通过深度强化学习有效生成关键场景的对抗性测试方法.

tags:
- 自动驾驶仿真
- 自动驾驶测试
- 自动驾驶汽车
- 智能网联汽车

# Display this page in the Featured widget?
featured: true

# links:
# - name: ""
#   url: ""
links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/378196389_Adversarial_Generation_of_Safety-Critical_Lane-Change_Scenarios_for_Autonomous_Vehicles

url_pdf: https://ieeexplore.ieee.org/document/10422684
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
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

 *下面为本研究的简介，详细内容请参阅[论文](https://ieeexplore.ieee.org/document/10422684)原文*

![avatar](./Fig_1.jpg)

---


## Citation
If you find our work is useful in your research, please consider citing:
```
@INPROCEEDINGS{10422684,
  author={He, Zimin and Zhang, Jiawei and Yao, Danya and Zhang, Yi and Pei, Huaxin},
  booktitle={2023 IEEE 26th International Conference on Intelligent Transportation Systems (ITSC)}, 
  title={Adversarial Generation of Safety-Critical Lane-Change Scenarios for Autonomous Vehicles}, 
  year={2023},
  volume={},
  number={},
  pages={6096-6101},
  keywords={Deep learning;Performance evaluation;Simulation;Reinforcement learning;Safety;Autonomous vehicles;Testing},
  doi={10.1109/ITSC57777.2023.10422684}}
```

