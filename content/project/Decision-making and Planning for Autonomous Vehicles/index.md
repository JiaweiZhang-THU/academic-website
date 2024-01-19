---
title: 自动驾驶汽车自主决策

summary: 本项目面向高级别自动驾驶技术需求，开展安全可信的自动驾驶汽车自主决策相关研究。考虑不同任务的特异性，分别提出了基于深度强化学习的路线规划算法、 基于多智能体的换道决策算法、自动驾驶汽车安全预警算法、以及基于深度模型的BEV数据融合预测算法，为实现安全、高效、协同、可信的智能驾驶提供了理论和技术支撑。

tags:
  - 自动驾驶
  - 智能汽车
  - 决策规划
  - 安全预警
  - BEV融合预测

date: '2023-06-23T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: route
    icon_pack: fas
    name: 自动驾驶路线规划
    url: https://ieeexplore.ieee.org/abstract/document/10221733
  - icon: road
    icon_pack: fas
    name: 自动驾驶换道决策
    url: https://ieeexplore.ieee.org/abstract/document/9932003
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
  + Paper: [A Bi-level Network-wide Cooperative Driving Approach Including Deep Reinforcement Learning-based Routing](https://ieeexplore.ieee.org/abstract/document/10221733)
  + Paper: [Self-Organized Routing for Autonomous Vehicles via Deep Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/10244078)
  
## 研究工作2：自动驾驶换道决策
  + Paper: [Multi-agent DRL-based lane change with right-of-way collaboration awareness](https://ieeexplore.ieee.org/abstract/document/9932003)
<img src=LaneChangeModel.jpg  width=60% />
  
## 研究工作3：自动驾驶安全预警
  + Paper: [Driving Safety Monitoring and Warning for Connected and Automated Vehicles via Edge Computing](https://ieeexplore.ieee.org/abstract/document/9922076)
  
## 研究工作4：自动驾驶BEV融合预测
  + Paper: [BEV-V2X: Cooperative Birds-Eye-View Fusion and Grid Occupancy Prediction via V2X-Based Data Sharing](https://ieeexplore.ieee.org/abstract/document/10179171)


## This project involves the following system components:

+ ### Cooperative Driving at Intersection with Deep Learning Model

  <img src="Intersection.gif" alt="Intersection" style="zoom:50%;" />

  

  + Paper: [Coordinating CAV Swarms at Intersections with A Deep Learning Model](https://jiaweizhang.netlify.app/publication/coordinating-cav-swarms-at-intersections-with-a-deep-learning-model/)
  
    ![avatar](./IntersectionModel.jpg)

---


+ ### Multi-agent DRL based Lane-Change

  <img src="LaneChange.gif" alt="LaneChange" style="zoom:50%;" />


  + Paper: [Multi-Agent DRL-based Lane Change with Right-of-Way Collaboration Awareness](https://jiaweizhang.netlify.app/publication/multi-agent-drl-based-lane-change-with-right-of-way-collaboration-awareness/)

    ![avatar](./LaneChangeModel.jpg)

---

+ ### Fault-tolerant cooperative driving at signal-free intersections

  <img src="faulteatIntersection.gif" alt="faulteatIntersection" style="zoom:120%;" />


  + Paper: [Fault-tolerant cooperative driving at signal-free intersections](https://jiaweizhang.netlify.app/publication/fault-tolerant-cooperative-driving-at-signal-free-intersections/)

    ![avatar](./faulteatIntersectionModel.jpg)
