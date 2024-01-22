---
title: "A bi-level network-wide cooperative driving approach including deep reinforcement learning-based routing"
authors:
- admin
- Jingwei Ge
- Shu Li
- Shen Li
- Li Li
author_notes:
date: "2023-08-17T00:00:00Z"
doi: "https://ieeexplore.ieee.org/document/10221733"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-08-17T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Vehicles*<br />(中科院1区; JCR Q1区; 影响因子=8.200)"
publication_short: "IEEE T-IV"

abstract: 针对自动驾驶路线规划问题面临的系统复杂、信息有限、决策耦合等挑战，本研究提出了基于深度强化学习的路线规划算法。通过创新的分层决策机制和自组织动态规划规划原则，以及新颖的深度强化学习路线规划模型，实现了前馈、主动高效的路线规划性能，显著提升了自动驾驶汽车的出行效率，同时协同提高了交通巨系统的运行效率。

# Summary. An optional shortened abstract.
summary: 一种新颖的基于深度强化学习的路线规划方法

tags:
- 路线规划
- 协同驾驶
- 无信号交叉口
- 深度强化学习
- 蒙特卡洛树搜索

featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/373162719_A_Bi-level_Network-wide_Cooperative_Driving_Approach_Including_Deep_Reinforcement_Learning-based_Routing

url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10221733
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

 *下面为本研究的简要介绍，详细内容请参阅[论文](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10221733)原文*

<img src=Fig_1.jpg  width=90% />

**分层决策机制**。在上层，我们提出了基于多智能体深度强化学习（DRL）的动态路线规划模型，其以宏观的交通状态信息为输入，输出介观的路线选择。在下层，我们提出了基于蒙特卡洛树搜索的交叉口协同驾驶算法，其以介观层的系统状态信息作为输入，输出微观路权调度结果，即通过冲突区域的车辆的通行权分配。

---
<img src=Fig_2.jpg  width=90% />

**分层决策规划框架**。

---
<img src=Fig_3.jpg  width=80% />

**自组织路线规划机制和本文构建的深度强化学习模型**。（*a*）自组织路线规划机制。路线规划按照“想三步，看两步，走一步”的原则展开。红色阴影车道是候选路线，蓝色阴影车道是与两条候选路线相对应的后续车道。绿色阴影区域上的交通状态信息是动态路线规划的关键。蓝色虚线路线表示到达目的地的候选路线的最短后续路线。（*b*）深度强化学习模型的观测空间，其中左侧子图为一步距离观测，右侧子图为两步距离观测。

---
<img src=Fig_4.jpg  width=60% />

**基于多智能体深度强化学习的路线规划模型训练**

---
<img src=Fig_5.jpg  width=90% />

**基于蒙特卡洛树搜索的交叉口自适应协同驾驶算法**。（*左*）交叉口车辆排队长度信息（由当前交叉口的路侧单元获得）和每条车道的驶入交通流量信息（由相邻交叉口的路侧单元和V2X通信获得）将用于确定控制区内车辆的路权分配（由蓝色虚线指示）。（*右*）通行证的说明。例如，“*BDEFCA*”是一个可行的传递顺序。当两辆车的路线冲突时，车辆在通过顺序中越靠前，其优先级就越高。比如，*Vehicle D*的优先级高于*Vehicle A*的优先级。

---
<img src=Fig_6.jpg  width=90% />

**基于蒙特卡洛树搜索的交叉口自适应协同驾驶算法**。MCTS算法：（*i*）选择：根据得分选择最有希望的节点；（*ii*）扩展：将未访问的子节点扩展到当前搜索树中；（*iii*）模拟：运行多轮次模拟，直到达到一个叶节点，即获得完整的路权分配；（*iv*）反向传播：根据叶节点的得分更新所有父节点的得分。

---
<img src=Fig_8.jpg  width=90% />

**性能**-不同到达率下车辆的出行耗时

---
<img src=Fig_9.jpg  width=90% />

**性能**-不同到达率下路网内的车辆累积量


---
<img src=Fig_10.jpg  width=60% />

**性能**-路网宏观基本图（Macroscopic fundamental diagram）结果

---
<img src=Fig_11.jpg  width=90% />

**不同方法下的模拟快照**：（*a*） 基准方法；（*b*） 本研究提出的方法。

---
<img src=Fig_12.jpg  width=70% />

**基于深度强化学习的路线规划模型训练**

---

## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10221733,
  author={Zhang, Jiawei and Ge, Jingwei and Li, Shu and Li, Shen and Li, Li},
  journal={IEEE Transactions on Intelligent Vehicles}, 
  title={A Bi-level Network-wide Cooperative Driving Approach Including Deep Reinforcement Learning-based Routing}, 
  year={2023},
  volume={},
  number={},
  pages={1-17},
  doi={10.1109/TIV.2023.3305818}
}
```

