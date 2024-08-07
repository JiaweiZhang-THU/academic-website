---
title: 智能网联汽车协同决策

summary: 本项目重点研究智能网联汽车协同决策理论与应用，针对典型场景下的协同决策问题，提出了基于深度学习模型的协同决策算法、基于深度强化学习的协同泊车算法、协同决策容错与自愈算法等先进方法，实现了大规模场景下实时求解、效率最优、安全可信、容错自愈的协同决策性能，为智能网联汽车技术的综合落地应用奠定了理论基础。

tags:
  - 智能网联汽车
  - 自动驾驶
  - 车辆群体协同驾驶
  - 决策规划
  - 群体机器人调度
  - 智能群系统容错自愈

date: '2022-12-24T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: car
    icon_pack: fas
    name: 车辆群体协同决策
    url: https://jiaweizhang.netlify.app/publication/coordinating-cav-swarms-at-intersections-with-a-deep-learning-model/
  - icon: robot
    icon_pack: fas
    name: 多机器人智能泊车
    url: https://jiaweizhang.netlify.app/publication/a-bi-level-cooperative-operation-approach-for-agv-based-automated-valet-parking/
  - icon: user-shield
    icon_pack: fas
    name: 智能群系统容错与自愈
    url: https://ieeexplore.ieee.org/abstract/document/9735412
  - icon: square-root-variable
    icon_pack: fas
    name: 协同决策理论研究
    url: https://jiaweizhang.netlify.app/publication/analysis-of-cooperative-driving-strategies-at-road-network-level-with-macroscopic-fundamental-diagram/
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
## 研究工作1：车辆群体协同决策
针对智能网联汽车协同决策面临的强交互、解空间巨大、强实时性等挑战，本研究提出基于深度模型的决策规划算法。该算法通过结合离线深度学习模型和在线蒙特卡洛树搜索，实现了求解速度最快、效率最优、规模最大的决策规划性能，比SOTA算法提高了55.6%。该研究为各类稀缺资源实时调度问题提供了通用的算法。详见该研究工作的[简介](https://jiaweizhang.netlify.app/publication/coordinating-cav-swarms-at-intersections-with-a-deep-learning-model/)。
  + 论文1: *Coordinating CAV swarms at intersections with a deep learning model* ([简介](https://jiaweizhang.netlify.app/publication/coordinating-cav-swarms-at-intersections-with-a-deep-learning-model/); [Paper](https://ieeexplore.ieee.org/abstract/document/10078727))
    
<img src=IntersectionModel.jpg  width=70% />

## 研究工作2：多机器人智能泊车
针对群体机器人泊车系统面临的调度规模巨大、决策耦合、低效死锁等挑战，本研究提出了基于深度强化学习的决策调度算法。该研究构建了智能分层决策系统，提出了群体机器人宏观任务调度、中观路线规划、微观协同决策、死锁监测自愈等一体化算法，显著提高了群体机器人的作业效率，任务平均耗时降低14%。详见该研究工作的[简介](https://jiaweizhang.netlify.app/publication/a-bi-level-cooperative-operation-approach-for-agv-based-automated-valet-parking/)。
  + 论文1: *A bi-level cooperative operation approach for AGV based automated valet parking* ([简介](https://jiaweizhang.netlify.app/publication/a-bi-level-cooperative-operation-approach-for-agv-based-automated-valet-parking/); [Paper](https://www.sciencedirect.com/science/article/pii/S0968090X21001583))
    
<img src=Parking.jpg  width=70% />
  
## 研究工作3：智能群系统容错与自愈
针对智能网联汽车面临的通信故障和机械故障，本研究提出了针对潜在故障的容错驾驶决策算法。该研究通过构建动态驾驶策略，实现了在保证安全的前提下，提高驾驶效率。作为最早将通信故障情况引入智能驾驶模型的研究，该研究解决了限制智能网联汽车发展的重大现实问题。详见该研究工作的[简介](https://jiaweizhang.netlify.app/publication/fault-tolerant-cooperative-driving-at-signal-free-intersections/)。
  + 论文1: *Fault-tolerant cooperative driving at signal-free intersections* ([简介](https://jiaweizhang.netlify.app/publication/fault-tolerant-cooperative-driving-at-signal-free-intersections/); [Paper](https://ieeexplore.ieee.org/abstract/document/9735412))
  + 论文2: *Fault-tolerant cooperative driving at highway on-ramps considering communication failure* ([简介](https://jiaweizhang.netlify.app/publication/fault-tolerant-cooperative-driving-at-highway-on-ramps-considering-communication-failure/); [Paper](https://www.sciencedirect.com/science/article/pii/S0968090X23002164))
  
<img src=Fault.jpg  width=70% />


## 研究工作4：协同决策理论研究
本研究对智能网联汽车协同决策问题开展了理论研究，分析了协同决策的内在机理，揭示了不同决策算法之间的本质区别，构建了以宏观基本图为核心的评估体系，验证了协同决策的瓶颈要素：二维路权冲突。该研究为智能网联汽车技术的进一步发展与应用指明了方向，具有重要的学术价值。详见该研究工作的[简介](https://jiaweizhang.netlify.app/publication/analysis-of-cooperative-driving-strategies-at-road-network-level-with-macroscopic-fundamental-diagram/)。
  + 论文1: *Analysis of cooperative driving strategies at road network level with macroscopic fundamental diagram* ([简介](https://jiaweizhang.netlify.app/publication/analysis-of-cooperative-driving-strategies-at-road-network-level-with-macroscopic-fundamental-diagram/); [Paper](https://www.sciencedirect.com/science/article/pii/S0968090X21004897))
  + 论文2: *Theoretical analysis of cooperative driving at idealized unsignalized intersections* ([简介](https://jiaweizhang.netlify.app/publication/theoretical-analysis-of-cooperative-driving-at-idealized-unsignalized-intersections/); [Paper](https://ieeexplore.ieee.org/abstract/document/10225295))
  
<img src=Analysis.jpg  width=70% />
