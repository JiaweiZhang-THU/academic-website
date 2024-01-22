---
title: "CAVSim: a microscopic traffic simulator for evaluation of connected and automated vehicles"
authors:
- admin
- Cheng Chang
- Zimin He
- Wenqin Zhong
- Danya Yao
- Shen Li
- Li Li
author_notes:
date: "2023-04-24T00:00:00Z"
doi: "10.1109/TITS.2023.3273565"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-04-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.551)"
publication_short: "IEEE T-ITS"

abstract: 针对自动驾驶仿真在前馈式决策规划、多车协同决策、基准场景算法、测试验证评估等方面的迫切需求，本工作研发了自动驾驶仿真测试平台CAVSim。该平台能够满足以上仿真需求，突出自动驾驶前馈式决策与规划，支持多车协同驾驶仿真。同时，该平台嵌入了丰富的协同决策场景、基准算法、测试功能，具有重要的研究和应用价值。该平台在开源后得到广泛应用，已有数十篇高水平学术论文基于该平台发表.

# Summary. An optional shortened abstract.
summary: 面向高级别自动驾驶技术的自动驾驶仿真平台.

tags:
- 自动驾驶仿真
- 自动驾驶测试
- 自动驾驶汽车
- 智能网联汽车
- 决策规划
- 微观交通仿真
- 车队稳定性测试


featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/370731657_CAVSim_A_Microscopic_Traffic_Simulator_for_Evaluation_of_Connected_and_Automated_Vehicles
url_pdf: https://ieeexplore.ieee.org/abstract/document/10124078
url_code: 'https://github.com/JiaweiZhang-THU/CAVSim'
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

## The overall framework of CAVSim.
![avatar](./Fig_2.jpg)

---
## The bi-level framework of cooperative driving for CAV swarms. 
![avatar](./Fig_4.jpg)

---
##  A typical signal-free intersection. 
#### For example, “*BDEFCA*” is a feasible passing order. When the routes of two vehicles conflict, the more  front the vehicle is in the passing order, the higher its priority. For example, the priority of *Vehicle D* is higher than the priority of *Vehicle A*.

![avatar](./Fig_5.jpg)

---
##  A typical on-ramp merging scenario for connected and automated vehicles.
![avatar](./Fig_6.jpg)

---
## The velocities of a CAV platoon under different cruise settings in CAVSim.
#### We simulate the scenario that the speed of the leading vehicle (i.e., *Vehicle 1*) suddenly decelerates from *20m/s* to *5m/s* under different settings.
![avatar](./Fig_7.jpg)

---
##  Vehicle trajectories at the on-ramp scenario under different cooperative driving algorithms.
![avatar](./Fig_14.jpg)





## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10124078,
  author={Zhang, Jiawei and Chang, Cheng and He, Zimin and Zhong, Wenqin and Yao, Danya and Li, Shen and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={CAVSim: A Microscopic Traffic Simulator for Evaluation of Connected and Automated Vehicles}, 
  year={2023},
  volume={},
  number={},
  pages={1-17},
  doi={10.1109/TITS.2023.3273565}
}
```

