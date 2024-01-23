---
title: "A bi-level cooperative operation approach for AGV based automated valet parking"
authors:
- admin
- Zhiheng Li
- Li Li
- Yidong Li 
- Hairong Dong
author_notes:
date: "2023-02-15T00:00:00Z"
doi: "https://doi.org/10.1016/j.trc.2021.103140"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-02-15T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*Transportation Research Part C: Emerging Technologies* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.022)"
publication_short: "TRC"

abstract: 针对多机器人智能泊车系统面临的调度问题规模巨大、不同层级决策耦合、低效死锁等挑战，本研究提出了基于深度强化学习的群体机器人调度系统及算法。该研究构建了新兴分层调度系统，提出了群体机器人宏观任务调度、中观路线规划、微观协同决策、死锁监测自愈等算法，大幅提高了机器人泊车系统的高效性、稳定性、协同性。本研究为群体机器人协同作业场景提供了一般性的调度系统及先进算法。

# Summary. An optional shortened abstract.
summary: 基于深度强化学习的群体机器人调度系统及算法

tags:
- 群体机器人
- 调度优化
- 深度强化学习
- 任务调度
- 路线规划
- 协同决策
- 协同泊车
- 死锁监测与自愈
featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/351661459_A_bi-level_cooperative_operation_approach_for_AGV_based_automated_valet_parking
url_pdf: https://www.sciencedirect.com/science/article/pii/S0968090X21001583
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
  - Cooperative Decision-making and Planning for Connected and Automated Vehicles

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

*下面为本研究的简要介绍，详细内容请参阅[论文](https://www.sciencedirect.com/science/article/pii/S0968090X21001583)原文*


<img src=Fig1.jpg  width=70% />

**典型的群体机器人停车系统**. 典型的群体机器人停车常，车辆在停车场中不断进出。司机在停车场入口或下车区下车。停车场作业管理（POM）系统为其分配未占用的停车位，然后AGV机器人将车辆运输到分配的停车位中。通常，一个大型停车场包含数百个停车位，并根据布局划分为几个区域。为了增加单个训练结果的可扩展性，期望不同区域的拓扑结构相似。同时，为了充分发挥大型停车场的优势，到达的车辆通常均匀分布在不同的区域，或者根据驾驶员距离目的地的远近，根据就近原则进行区域分配。

---

<img src=Fig2.jpg  width=95% />

**我们提出的多AGV机器人泊车调度系统**. 系统分为任务调度、路线规划和轨迹规划。任务调度根据停车场的情况为到达的车辆分配停车位。给定地图和分配的停车位，路线规划通过避开静态障碍物来确定到达目的地的路线。轨迹规划计算纵向轨迹以遵循路线，同时避免碰撞和死锁。与上述三个子模块并行的另一个子模块是死锁检测和自愈模块，用于检测潜在的环形死锁并恢复锁定的机器人。

---

<img src=Fig3.jpg  width=50% />

**基于深度强化学习的任务调度模型之状态空间设置**

---

<img src=Fig4.jpg  width=50% />

**基于深度强化学习的任务调度模型**. 使用深度强化学习算法解决全局停车位分配问题主要有以下困难：（*i*）奖励是稀疏的，大多数随机选择的经验对模型学习的贡献很小；（*ii*） 即使在模拟环境中，对状态-动作空间的探索也是耗时的；（*iii*） 环境是动态的，许多随机因素（如车辆到达和离开时间的不确定性等）干扰模型训练，这使得事件奖励的方差很大。为了应对上述挑战，我们提出了一种基于原始深度Q网络（DQN）和现有改进技术的Double Dueling Deep Q-network。


---

<img src=Fig5.jpg  width=50% />

**基于深度强化学习的任务调度模型之深度网络设置**

---


## Citation
If you find our work is useful in your research, please consider citing:
```
@article{zhang2021bi,
  title={A bi-level cooperative operation approach for AGV based automated valet parking},
  author={Zhang, Jiawei and Li, Zhiheng and Li, Li and Li, Yidong and Dong, Hairong},
  journal={Transportation Research Part C: Emerging Technologies},
  volume={128},
  pages={103140},
  year={2021},
  publisher={Elsevier}
}
```

