---
title: "Driving safety monitoring and warning for connected and automated vehicles via edge computing"
authors:
- Cheng Chang
- Kunpeng Zhang
- admin
- Shen Li
- Li Li
author_notes:
date: "2022-10-08T00:00:00Z"
doi: "10.1109/ITSC55140.2022.9922076"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-08T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*2022 IEEE 25th International Conference on Intelligent Transportation Systems (ITSC)*"
publication_short: "IEEE ITSC"

abstract: In this paper, we systematically study how to use edge computing to monitor the movements of multiple connected and automated vehicles (CAV) and warn of potential accidents (e.g., lane departures, collisions). Compared to conventional approaches that only use the sensing data of individual vehicles, cooperative vehicle infrastructure systems directly collect the movement data of vehicles via vehicle-to-everything (V2X) communications and thus easily calculate the risk of every vehicle synthetically. We propose a fast algorithm and the corresponding data structure model to calculate collision risks based on the timely received data. We also discuss the data accuracy and transmission delay requirements to guarantee the driving safety of CAVs. Testing results show the effectiveness of the proposed approach.

# Summary. An optional shortened abstract.
summary: 基于边缘计算的自动驾驶安全监测与预警算法.

tags:
- Cooperative Driving
- Driving Safety Monitoring
- Driving Safety Warning
- Connected and Automated Vehicle
# Display this page in the Featured widget?
featured: true

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/364998087_Driving_Safety_Monitoring_and_Warning_for_Connected_and_Automated_Vehicles_via_Edge_Computing
url_pdf: https://ieeexplore.ieee.org/abstract/document/9922076
url_code: ''
url_dataset: ''
url_poster: ''
url_project: https://jiaweizhang.netlify.app/project/decision-making-and-planning-for-autonomous-vehicles/
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
本研究旨在探索如何利用边缘计算技术提高自动驾驶的安全性。通过V2X通信技术，我们能够收集车辆的运动数据，并综合评估每辆车的潜在风险，从而有效预警车道偏离、碰撞等危险情况。

我们提出了一个创新的框架，该框架包含快速算法和数据结构模型，用以实时计算碰撞风险。框架的核心在于使用CD-DB数据结构存储车辆数据，并通过额外的指针优化历史轨迹数据的查询效率。我们还开发了三种不同的轨迹预测算法，分别适用于不同自动化水平的车辆，以及一个快速的线段相交判断算法用于碰撞检测。

此外，我们还设计了一个预警算法，它根据车辆的类型和状态确定预警，并生成包含即将碰撞对象的当前状态信息的数据包。这些数据包通过V2X通信协议传输给车辆，指导车辆进行避险操作。

通过一系列模拟测试，我们验证了所提出方法的有效性。测试结果表明，我们的系统能够在保持高TPR的同时，有效降低误报率（FPR），并且在处理速度上也达到了可接受的水平。与传统的单个车辆预警方法相比，基于边缘计算的预警方法表现出更好的性能。我们的研究表明，边缘计算技术在提升CAV驾驶安全性方面具有巨大潜力。

 *下面为本研究的简介，详细内容请参阅[论文](https://ieeexplore.ieee.org/abstract/document/9922076)原文*

![avatar](./Fig_1.jpg)

---

![avatar](./Fig_0.jpg)

---

## Citation
If you find our work is useful in your research, please consider citing:
```
@INPROCEEDINGS{9922076,
  author={Chang, Cheng and Zhang, Kunpeng and Zhang, Jiawei and Li, Shen and Li, Li},
  booktitle={2022 IEEE 25th International Conference on Intelligent Transportation Systems (ITSC)}, 
  title={Driving Safety Monitoring and Warning for Connected and Automated Vehicles via Edge Computing}, 
  year={2022},
  volume={},
  number={},
  pages={3940-3947},
  doi={10.1109/ITSC55140.2022.9922076}}

```

