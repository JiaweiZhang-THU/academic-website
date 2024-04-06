---
title: 自动驾驶汽车自主决策

summary: 本项目面向高级别自动驾驶技术需求，开展安全可信的自动驾驶汽车自主决策相关研究。考虑不同任务的特异性，分别提出了基于深度强化学习的路线规划算法、 基于多智能体的换道决策算法、自动驾驶汽车安全预警算法、以及基于深度模型的BEV数据融合预测算法，为实现安全、高效、协同、可信的智能驾驶提供了理论和技术支撑。

tags:
  - 自动驾驶
  - 智能汽车
  - 决策规划
  - 安全预警
  - BEV融合预测

date: '2022-12-25T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: route
    icon_pack: fas
    name: 自动驾驶路线规划
    url: https://jiaweizhang.netlify.app/publication/a-bi-level-network-wide-cooperative-driving-approach-including-deep-reinforcement-learning-based-routing/
  - icon: road
    icon_pack: fas
    name: 自动驾驶换道决策
    url: https://jiaweizhang.netlify.app/publication/multi-agent-drl-based-lane-change-with-right-of-way-collaboration-awareness/
  - icon: car-burst
    icon_pack: fas
    name: 自动驾驶安全预警
    url: https://ieeexplore.ieee.org/abstract/document/9922076
  - icon: car
    icon_pack: fas
    name: BEV感知融合与预测
    url: https://ieeexplore.ieee.org/abstract/document/10179171
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
## 研究工作1：自动驾驶路线规划
针对自动驾驶路线规划问题面临的系统复杂、信息有限、决策耦合等挑战，本研究提出了基于深度强化学习的路线规划算法。通过创新的分层决策机制和自组织动态规划规划原则，以及新颖的深度强化学习路线规划模型，实现了前馈、主动高效的路线规划性能，显著提升了自动驾驶汽车的出行效率，同时协同提高了交通巨系统的运行效率。详将该研究工作的[简介](https://jiaweizhang.netlify.app/publication/a-bi-level-network-wide-cooperative-driving-approach-including-deep-reinforcement-learning-based-routing/)。
  + 论文1: *A bi-level network-wide cooperative driving approach including deep reinforcement learning-based routing* ([简介](https://jiaweizhang.netlify.app/publication/a-bi-level-network-wide-cooperative-driving-approach-including-deep-reinforcement-learning-based-routing/); [Paper](https://ieeexplore.ieee.org/abstract/document/10221733))
  + 论文2: *Self-organized routing for autonomous vehicles via deep reinforcement learning* ([简介](https://jiaweizhang.netlify.app/publication/self-organized-routing-for-autonomous-vehicles-via-deep-reinforcement-learning/); [Paper](https://ieeexplore.ieee.org/abstract/document/10244078))

<img src=Routing.jpg  width=90% />

## 研究工作2：自动驾驶换道决策
针对智能驾驶决策任务中的强交互、多目标、机理模糊等挑战，本研究提出了首个基于多智能体深度强化学习的换道决策算法。通过安全可信的复合决策框架、全新的多智能体决策模型、基于行为意图的状态信息编码，突破了单智能体决策范式的性能瓶颈，自动驾驶行车效率提高9%、安全性提高70%，并涌现出群体协同智能。详将该研究工作的[简介](https://jiaweizhang.netlify.app/publication/multi-agent-drl-based-lane-change-with-right-of-way-collaboration-awareness/)。
  + 论文1: *Multi-agent DRL-based lane change with right-of-way collaboration awareness* ([简介](https://jiaweizhang.netlify.app/publication/multi-agent-drl-based-lane-change-with-right-of-way-collaboration-awareness/); [Paper](https://ieeexplore.ieee.org/abstract/document/9932003))
    
<img src=LaneChangeModel.jpg  width=90% />

## 研究工作3：自动驾驶安全预警
针对自动驾驶安全监测预警面临的预警范围有限、预警不及时、虚警率高等挑战，本研究提出了基于边缘计算的自动驾驶安全监测与预警算法。该算法通过全新的安全预警框架和基于深度模型的车辆轨迹预测，实现了更全面、更可信、更及时的自动驾驶安全监测与预警，预警命中率超过80%，为当前性能最佳。详将该研究工作的[简介](https://jiaweizhang.netlify.app/publication/driving-safety-monitoring-and-warning-for-connected-and-automated-vehicles-via-edge-computing/)。
  + 论文1: *Driving safety monitoring and warning for connected and automated vehicles via edge computing* ([简介](https://jiaweizhang.netlify.app/publication/driving-safety-monitoring-and-warning-for-connected-and-automated-vehicles-via-edge-computing/); [Paper](https://ieeexplore.ieee.org/abstract/document/9922076))
    
<img src=Safety.jpg  width=90% />

## 研究工作4：自动驾驶BEV融合预测
针对自动驾驶鸟瞰图(Birds-Eye-View, BEV)感知任务面临的信息不准确、范围不足、可解释性差等挑战，本研究提出了基于V2X的BEV数据融合预测模型。该模型基于注意力神经网络，实现了感知范围更广、预测精度更高、可解释性更强的BEV融合与预测性能。该模型突破了现有的单车BEV融合模型的性能瓶颈，预测准确性提高超过15%。详将该研究工作的[简介](https://jiaweizhang.netlify.app/publication/bev-v2x-cooperative-birds-eye-view-fusion-and-grid-occupancy-prediction-via-v2x-based-data-sharing/)。
  + 论文1: *BEV-V2X: cooperative Birds-Eye-View fusion and grid occupancy prediction via V2X-based data sharing* ([简介](https://jiaweizhang.netlify.app/publication/bev-v2x-cooperative-birds-eye-view-fusion-and-grid-occupancy-prediction-via-v2x-based-data-sharing/); [Paper](https://ieeexplore.ieee.org/abstract/document/10179171))
    
<img src=BEV.jpg  width=90% />

