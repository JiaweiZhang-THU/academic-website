---
title: "Multi-agent DRL-based lane change with right-of-way collaboration awareness"
authors:
- admin
- Cheng Chang
- Xianlin Zeng
- Li Li
author_notes:
date: "2023-01-02T00:00:00Z"
doi: "10.1109/TITS.2022.3216288"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-01-02T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.551)"
publication_short: "IEEE T-ITS"

abstract: 针对智能驾驶自主换道任务中的强交互、多目标、机理模糊等挑战，本研究提出了基于多智能体深度强化学习的换道决策算法。该算法通过安全可信的复合决策框架，将其他车辆的行为意图纳入自车决策，突破了传统的单智能体范式的性能瓶颈，显著提升了自动驾驶的安全性、高效性、协同性，并在宏观层涌现出群体协同智能。

# Summary. An optional shortened abstract.
summary: 首个多智能体换道算法，突破传统的单智能体算法的性能瓶颈.

tags:
- 自动驾驶
- 决策规划
- 换道决策
- 路权分配
- 多智能体
- 深度强化学习
- 驾驶意图
- 行为意图
- 协同驾驶
- 
featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/364828330_Multi-Agent_DRL-Based_Lane_Change_With_Right-of-Way_Collaboration_Awareness
url_pdf: https://ieeexplore.ieee.org/abstract/document/9932003
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
  - Decision-making and Planning for Autonomous Vehicles

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
#### The overall architecture of the proposed bi-level lane-change behavior planning strategy.
![avatar](./featured.jpg)
---

#### An illustration of the traffic snapshot and driving intention.
![avatar](./Fig_2.jpg)
---

#### The training pipeline of the upper-level SAC based lane-change decision model.
![avatar](./Fig_3.jpg)

---

## Performance

#### Average speed of traffic flow under different lane-change decision models. The baseline denotes that lane changes are not allowed and all vehicles keep the lanes.
![avatar](./Fig_4.jpg)
---


#### Screenshot of the traffic simulation, where we enable only the upper-level lane-change decision model but do not enable the lower-level right-ofway assignment model. *Vehicle A* and *Vehicle B* collide during executing the lane-change actions.
![avatar](./Fig_11.jpg)

---

#### Screenshot of traffic simulation with the proposed bi-level lanechange behavior planning strategy. The lower-level right-of-way assignment model avoids the potential collision between *Vehicle C* and *Vehicle D*.
![avatar](./Fig_12.jpg)

---

#### Vehicle trajectories in congested traffic with different lane-change decision models. The upper subfigure is from the model that only considers ego benefits, and the lower subfigure is from the proposed model.
![avatar](./Fig_14.jpg)

---




## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{9932003,
  author={Zhang, Jiawei and Chang, Cheng and Zeng, Xianlin and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={Multi-Agent DRL-Based Lane Change With Right-of-Way Collaboration Awareness}, 
  year={2023},
  volume={24},
  number={1},
  pages={854-869},
  doi={10.1109/TITS.2022.3216288}
}
```

