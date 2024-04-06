---
title: 自动驾驶技术仿真测试
summary: 本项目重点研究自动驾驶仿真和测试相关课题，针对高级别智能驾驶系统仿真测试需求，研发了自动驾驶开源仿真平台，提出了自动驾驶智能测试方法和测试场景生成方法，并开发了自动驾驶实车系统，为高级别自动驾驶技术的研发、仿真、测试提供了平台与方法支撑。

tags:
  - 自动驾驶仿真
  - 智能测试
  - 实车系统
  - 智能网联汽车
  - 场景生成

date: '2022-12-23T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: network-wired
    icon_pack: fas
    name: 自动驾驶仿真平台
    url: https://jiaweizhang.netlify.app/publication/cavsim-a-microscopic-traffic-simulator-for-evaluation-of-connected-and-automated-vehicles/
  - icon: truck-fast
    icon_pack: fas
    name: 自动驾驶实车系统
    url: https://github.com/JiaweiZhang-THU/CAVSim
  - icon: road-circle-check
    icon_pack: fas
    name: 自动驾驶智能测试
    url: https://ieeexplore.ieee.org/abstract/document/10130026
  - icon: truck-moving
    icon_pack: fas
    name: 自动驾驶场景生成
    url: https://ieeexplore.ieee.org/abstract/document/10401017
  

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


## 研究工作1：自动驾驶仿真平台
针对高级别自动驾驶仿真测试需求，本工作研发了自动驾驶仿真平台CAVSim。相较于其他平台，该平台是首个支持智能网联汽车协同决策和自动驾驶前馈式决策规划的仿真平台，提供了丰富的决策规划基准算法和测试功能。该平台由本人主导研发，C++代码量超一万行，已有数十篇高水平学术论文基于该平台发表。详见该研究工作的[简介](https://jiaweizhang.netlify.app/publication/cavsim-a-microscopic-traffic-simulator-for-evaluation-of-connected-and-automated-vehicles/)。
  + 论文1: *CAVSim: a microscopic traffic simulator for evaluation of connected and automated vehicles* ([简介](https://jiaweizhang.netlify.app/publication/cavsim-a-microscopic-traffic-simulator-for-evaluation-of-connected-and-automated-vehicles/); [Paper](https://ieeexplore.ieee.org/abstract/document/10124078))
  + 论文2: *CAVSim: A Microscope Traffic Simulator for Connected and Automated Vehicles Environment* ([简介](https://jiaweizhang.netlify.app/publication/cavsim-a-microscope-traffic-simulator-for-connected-and-automated-vehicles-environment/); [Paper](https://ieeexplore.ieee.org/abstract/document/9922267))
  + Code: [CAVSim](https://github.com/JiaweiZhang-THU/CAVSim)

<img src=CAVSim_Architecture.jpg  width=70% />
<img src="Cooperative Driving at Signal-free Intersections_1.gif" alt="Cooperative Driving at Signal-free Intersections_1" style="zoom:70%;" />

## 研究工作2：自动驾驶实车系统
    作为主要贡献者，本人参与研发了智能网联汽车实车系统，完成了典型场景下的智能网联汽车协同决策系统、车辆轨迹规划系统、安全监测预警系统的技术突破和工程实现。在国家智能汽车与智慧交通示范基地开展10辆智能网联汽车协同驾驶的实验验证工作。
<img src="RealVehicle.gif" alt="Autonomous driving real vehicle system" style="zoom:70%;" />
  
## 研究工作3：自动驾驶智能测试算法
智能测试对于自动驾驶技术的部署应用至关重要，其中如何高效构建关键测试场景是自动驾驶智能测试的核心。本研究提出了一种基于深度强化学习的对抗测试方法，该方法通过构建对抗智能体和创新模型奖励函数，兼顾了测试场景的关键性和真实性，实现了更高效且更符合真实场景的自动驾驶智能测试。
  + 论文: *Adversarial Generation of Safety-Critical Lane-Change Scenarios for Autonomous Vehicles* ([Paper](https://ieeexplore.ieee.org/document/10422684))
    
<img src=AdversarialTesting.jpg  width=70% />

## 研究工作4：高级别自动驾驶大规模部署
针对智能驾驶技术在混行交通中的应用挑战，本研究提出了自动驾驶专用道路策略，该策略能够实现人车和自动驾驶汽车的智能分流，为高级别智能驾驶技术的大规模部署应用提供了方案。我们构建了专用路权部署模型，提出了基于群体智能的部署算法，以及车辆群体路线规划方法，在实现智能分流的同时，自动驾驶车辆出行效率提高11%。
  + 论文1: *Unleashing the power of connected and automated vehicles: A dedicated link strategy for efficient management of mixed traffic* ([简介](https://jiaweizhang.netlify.app/publication/unleashing-the-power-of-connected-and-automated-vehicles-a-dedicated-link-strategy-for-efficient-management-of-mixed-traffic/); [Paper](https://ieeexplore.ieee.org/document/10462009))
  + 论文2: *Unleashing the two-dimensional benefits of connected and automated vehicles via dedicated intersections in mixed traffic* ([简介](https://jiaweizhang.netlify.app/publication/unleashing-the-two-dimensional-benefits-of-connected-and-automated-vehicles-via-dedicated-intersections-in-mixed-traffic/); [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0968090X24000226))
  
<img src=DedicatedLink.jpg  width=70% />

