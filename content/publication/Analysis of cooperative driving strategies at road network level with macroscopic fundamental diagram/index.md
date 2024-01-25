---
title: "Analysis of cooperative driving strategies at road network level with macroscopic fundamental diagram"
authors:
- admin
- Huaxin Pei
- Xuegang (Jeff) Ban
- Li Li
author_notes:
date: "2023-1-01T00:00:00Z"
doi: "10.1016/j.trc.2021.103503"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*Transportation Research Part C: Emerging Technologies* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.551)"
publication_short: "TRC"

abstract: 本研究对智能网联汽车协同决策问题开展了理论研究，分析了协同决策的内在机理，揭示了不同协同决策算法之间的本质区别，构建了以宏观基本图为核心的评估方法，验证了协同决策的瓶颈要素：二维路权冲突，提出了统一的拉链式协同决策算法框架。该研究为协同决策技术的进一步发展指明了方向，具有重要意义。

# Summary. An optional shortened abstract.
summary: 提出车辆群体“宏观-中观-微观”系统机理与分层管控路线，分析验证了车辆群体协同决策的核心问题.

tags:
- 智能网联汽车
- 自动驾驶
- 理论研究
- 协同驾驶
- 宏观基本图
- 交通控制
- 路权分配
featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/357067155_Analysis_of_cooperative_driving_strategies_at_road_network_level_with_macroscopic_fundamental_diagram
url_pdf: https://www.sciencedirect.com/science/article/pii/S0968090X21004897
url_code: ''
url_dataset: ''
url_poster: ''
url_project: https://jiaweizhang.netlify.app/project/cooperative-decision-making-and-planning-for-connected-and-automated-vehicles/
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
  - Cooperative Decision-making and Planning for Connected and Automated Vehicles

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

 *下面为本研究的简要介绍，详细内容请参阅[论文](https://www.sciencedirect.com/science/article/pii/S0968090X21004897?via%3Dihub)原文*


<img src=Fig1.jpg  width=60% />

**A typical isolated intersection and an illustration of the passing order.** Vehicles A, B, C, and F will pass through the intersection. Order AFBCmeans that A, F, B, and C will pass through the conflict zone successively. In particular, it should be noted that some vehicles do not have conflicting paths, and thus they can drive into conflict zone simultaneously. Therefore, the order *AFBC* and *FABC* are essentially equivalent.

---

<img src=Fig2.jpg  width=60% />

Structure of a well-defined MFD

---

<img src=Fig3.jpg  width=95% />

Overview of the simulation platform

---

<img src=Fig4.jpg  width=60% />

A local intersection in the traffic network, where intersection conflict zone is decomposed to improve space utilization.

---

<img src=Fig5.jpg  width=60% />

The simulated two-lane road network with four intersections.

---

<img src=Fig6.jpg  width=95% />

MFDs of the network traffic under different control strategies.

---

<img src=Fig7.jpg  width=95% />

Average stopping time for different vehicle accumulations with different intersection control strategies. The left subfigure shows the average time of full stopping of the vehicles; the right shows the average time when the vehicle speed is less than 2m/s, i.e., slow-moving.

---

<img src=Fig8.jpg  width=195% />

The intersection throughput and network-wide outflow under different control strategies. The throughput in the upper subfigure is the average number of vehicles passing through a single intersection per minute, and the outflow in the lower subfigure is the average traffic flow at the network exit links.

---

<img src=Fig9.jpg  width=95% />

The accumulation of vehicles in the road network and the intersection control zone for different vehicle arrival rates, where the latter is the average vehicle accumulation at the four intersections within the network.

---

<img src=Fig10.jpg  width=95% />

A snapshot of the simulation platform under FIFO based cooperative driving strategy.

---

<img src=Fig11.jpg  width=95% />

The average travel time of vehicles in two typical routes, where travel time is defined as the time of vehicles from entering to leaving the boundary of the considered road network. The length of the red route is about 900 m, and the length of the green route is about 1000 m.

---

<img src=Fig12.jpg  width=95% />

The MFDs of network traffic with different car-following headway settings. The left subfigure corresponds to the MCTS based cooperative driving strategy, and the right subfigure corresponds to the FIFO based cooperative driving strategy. The FIFO baseline in the left subfigure is the average of the four FIFO curves in the right subfigure, and the MCTS baseline in the right subfigure is the average of the four MCTS curves in the left subfigure.

---

<img src=Fig13.jpg  width=50% />

The statistical zone used to count the gap between successive vehicles in the road network, where the length of the zone is 200 m.

---

<img src=Fig14.jpg  width=95% />

The distribution of the gap distance under different vehicle accumulation.

---

<img src=Fig15.jpg  width=95% />

Two typical heterogeneous traffic demand patterns. The traffic demand of the entrances indicated by the red arrows will be two or three times that of the entrances indicated by green arrows.

---

<img src=Fig16.jpg  width=95% />

MFDs of network traffic under different turning ratios. Turning #Pattern A in the left subfigure: the proportion of left-turning vehicles is 1/3, straight-traveling is 1/3, and the right-turning is 1/3. Turning #Pattern B in the right subfigure: the proportion of left-turning vehicles is 1/4, straight-traveling is 1/2, and right-turning is 1/4.

---

<img src=Fig17.jpg  width=60% />

A typical urban traffic network with twenty-five intersections. All straight links are 500 m long.

---

<img src=Fig18.jpg  width=60% />

MFDs of the traffic network with twenty-five intersections under different control strategies.

---

**仿真视频**

<img src="25VehicleData_603864_fps_100.gif" alt="Signal-free road network traffic" style="zoom:95%;" />

---

## Citation
If you find our work is useful in your research, please consider citing:
```
@article{ZHANG2022103503,
  title = {Analysis of cooperative driving strategies at road network level with macroscopic fundamental diagram},
  journal = {Transportation Research Part C: Emerging Technologies},
  volume = {135},
  pages = {103503},
  year = {2022},
  issn = {0968-090X},
  doi = {https://doi.org/10.1016/j.trc.2021.103503},
  url = {https://www.sciencedirect.com/science/article/pii/S0968090X21004897},
  author = {Jiawei Zhang and Huaxin Pei and Xuegang (Jeff) Ban and Li Li},
  keywords = {Cooperative driving, Network traffic, Passing order, Macroscopic fundamental diagram (MFD)}
}

```

