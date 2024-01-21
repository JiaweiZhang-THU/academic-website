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
    url: https://ieeexplore.ieee.org/abstract/document/10124078
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
[CAVSim](https://github.com/JiaweiZhang-THU/CAVSim) is a microscopic traffic simulator for the CAV environment. The framework of CAVSim is consistent with the realistic CAV environment, including module decomposition, road segmentation, computing task allocation, which can be conveniently used to deploy and test the cooperative driving methods at different levels about CAVs. Meanwhile, CAVSim emphasizes the critical properties and driving behaviors of CAVs and is dedicated to capturing the characteristics of CAVs and their impact on traffic flow. Modular development makes CAVSim have good scalability, which can simulate typical local traffic scenarios, and can also simulate large-scale network-wide traffic through reasonable splicing of road blocks. With CAVSim, users can conduct various traffic and vehicle simulations related to CAVs. Finally, CAVSim is an evolving project, and we will further refine and enhance it next. In particular, we will develop more benchmarking algorithms in CAVSim to promote the development of CAV with a unified platform.

## The overall framework of CAVSim.
![avatar](./Architecture.jpg)

---
#### **Lane Change at Straight Lane**
  <img src="Straight Lane.gif" alt="Straight Lane" style="zoom:90%;" />

---
#### **Cooperative Driving at Signal-free Intersections**

  <img src="Cooperative Driving at Signal-free Intersections_1.gif" alt="Cooperative Driving at Signal-free Intersections_1" style="zoom:90%;" />

---
#### **Multi-Vehicle Merging at On-ramps**

  <img src="Multi-CAV Merging at On-ramps.gif" alt="Multi-CAV Merging at On-ramps" style="zoom:80%;" />


---
#### **Simulation of Road Network Traffic**

  <img src="Network-wide Traffic Simualtion.gif" alt="Network-wide Traffic Simualtion" style="zoom:100%;" />


---

## Related Papers
+ [CAVSim: A Microscopic Traffic Simulator for Evaluation of Connected and Automated Vehicles](https://jiaweizhang.netlify.app/publication/cavsim-a-microscopic-traffic-simulator-for-evaluation-of-connected-and-automated-vehicles/)

#### Citation
```
@ARTICLE{Zhang2023CAVSim,
  title={CAVSim: A Microscopic Traffic Simulator for Evaluation of Connected and Automated Vehicles},
  author={Zhang, Jiawei and Chang, Cheng and He, Zimin and Zhong, Wenqin and Yao, Danya and Li, Shen and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems},
  year={2023},
  pages={1-17},
  doi={10.1109/TITS.2023.3273565},
  publisher={IEEE}
}
```
+ [CAVSim: A Microscope Traffic Simulator for Connected and Automated Vehicles Environment](https://jiaweizhang.netlify.app/publication/cavsim-a-microscope-traffic-simulator-for-connected-and-automated-vehicles-environment/)

#### Citation
```
@INPROCEEDINGS{Zhang2022CAVSim,
  author={Zhang, Jiawei and Chang, Cheng and Pei, Huaxin and Peng, Xinyu and Guo, Yuqing and Lian, Renzong and Chen, Zhenwu and Li, Li},
  booktitle={2022 IEEE 25th International Conference on Intelligent Transportation Systems (ITSC)}, 
  title={CAVSim: A Microscope Traffic Simulator for Connected and Automated Vehicles Environment}, 
  year={2022},
  pages={3719-3724},
  doi={10.1109/ITSC55140.2022.9922267},
  publisher={IEEE}
}
```
