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
doi: "10.1109/TIV.2023.3305818"

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

**性能-不同到达率下车辆的出行耗时**. 我们统计了不同到达率下车辆在等长路线上的行驶时间，结果如上图所示。结果表明，当到达率较低（例如，300veh/（h*lane））时，由于车辆数量较少且路网内交通顺畅，不同方法的性能相似。然而，随着到达率的增加，基准方法的旅行时间显著增加。同时，不同车辆的行驶时间差异很大。相反，在所提出的方法下，随着到达率的增加，车辆的行驶时间保持在较低的水平，同时，不同车辆行驶时间的差异较小。这表明，本文提出的路线规划方法减少了车辆的行驶时间，提高了整个路网交通系统的效率。此外，该方法具有较好的公平性，不同车辆的行驶时间方差较小。

---
<img src=Fig_9.jpg  width=90% />

**性能-不同到达率下路网内的车辆累积量**. 其次，我们统计了不同到达率下车辆在路网中的车辆累积情况，结果如上图所示。结果表明，在几乎所有到达率下，该方法都能实现较低的车辆累积。这表明，在所提出的方法下，车辆可以更有效地通过道路网络，从而使车辆在道路网络中的积累保持在较低的水平。此外，随着到达率的增加，在所提出的方法下，车辆累积的增加率小于基准方法。特别是当到达率为360veh/（h*车道）时，在基准方法下，路网很快就会失去平衡，即输出流量小于输入流量，车辆积累持续增加。相反，在所提出的方法下，全网流量系统仍然平稳运行。


---
<img src=Fig_10.jpg  width=60% />

**性能-路网宏观基本图（Macroscopic fundamental diagram）**. 第三，我们通过改变到达率来计算两种方法下整个路网的宏观基本图MFD，结果如上图所示。MFD结果表明，在较低的车辆累积量下，两种方法之间的差异并不显著。然而，随着车辆数量的增加，本文提出的方法可以实现更大的交通流量，这显著提高了交通系统的效率。此外，在我们的方法下，路网的MFD临界密度增加了，这表明本文的方法提高了路网的承载能力。

---
<img src=Fig_11.jpg  width=90% />

**不同方法下的模拟快照**：（*a*） 基准方法；（*b*） 本研究提出的方法。在这里，我们直观地展示了所提出的方法对性能的贡献。为此，我们在不同的方法下以相同的到达速率截取同一时刻的仿真快照，如上图所示。结果表明，在所提出的方法下，车辆在路网中的分布相对均匀和分散。同时，在局部交叉口，不同方向的车辆数量基本一致，不存在排队拥堵。相反，在基准方法下，道路网络内的车辆分布是不均衡的。十字路口不同方向的车辆数量差异很大，一些方向出现拥堵排队。

---
<img src=Fig_12.jpg  width=70% />

**基于深度强化学习的路线规划模型训练——状态空间**. 在这里，我们分析了所提出的两种类型的观测信息对路线规划模型的影响。上图显示了不同观察信息设置下奖励值随学习步骤的变化曲线。结果表明，在我们的观测空间设置下，所提出的路线规划模型获得了更高、更稳定的奖励值曲线。没有一步观测信息或两步观测信息的模型性能显著下降。特别是，结果表明，一步观测信息发挥了更大的主导作用，而两步观测信息对获得更高的回报做出了重要贡献。因此，本文提出的两种类型的观测信息对路线规划模型的性能有很大贡献。

---
<img src=Table2.jpg  width=70% />

**基于深度强化学习的路线规划模型训练——奖励函数**. 为了验证本文提出的基于背压的奖励函数的优越性，我们将其与基于行程时间的奖励函数进行了比较。基于行程时间的奖励是对路线决策的直接和绝对的性能评估。在这里，我们使用上述两种不同的奖励函数在相同的模拟环境中训练基于DRL的路线规划模型，其中训练期间车辆的到达率为400veh/（lane*h）。对于训练好的模型，我们在不同的到达率下对其进行了测试，结果如表II所示。结果表明，本文提出的基于反压的奖励函数使基于多智能体DRL的路线规划模型具有更好的性能，尤其是更好的泛化性能。当测试环境与训练环境不一致时，我们的模型可以获得更好的性能。其中一个关键原因是基于反压的奖励函数是对路线决策进行相对评估。无论是在交通顺畅还是拥堵的情况下，如果模型选择了更好的路线，它都会得到积极的奖励。相反，在平稳和拥堵的交通中，出行时间变化很大，因此基于出行时间的奖励函数不能准确反映路由决策所带来的性能。因此，研究结果表明，本文提出的基于背压的奖励函数有利于学习基于多智能体DRL的路由模型的期望性能，尤其是优异的泛化性能。


---
<img src=Fig_13.jpg  width=70% />

**路线规划模型的性能**. 我们将基于DRL的路线规划方法与基于Dijkstra的最短路线规划方法进行比较。在相同的交通需求下，我们分别部署了基于DRL的路线规划方法和基于Dijkstra的路线规划方法，并统计了车辆在相同路线上的行驶时间。结果如上图所示。结果表明，与基于Dijkstra的路线规划方法相比，所提出的基于DRL的路线规划方法在不同到达速率下可以实现更短的行程时间。随着到达率的增加，所提出的基于DRL的路线规划方法的性能优势变得更加显著，并且出行耗时缓慢增加。相反，在基于Dijkstra的路线规划方法下，出行耗时随着到达率的增加而显著增加。

---

*下面为微观层的交叉口自适应协同驾驶方法的性能评估*

<img src=Fig_14.jpg  width=70% />

**蒙特卡洛树搜索的关键参数**. 我们通过将w_{Pr}和η从0变为1来获得性能改进结果。结果表明，在大多数参数设置情况下，自适应协同驾驶算法具有显著的性能提高，缩短了车辆的平均行驶时间。其中，当w_{Pr}为0.8，η为0.4时，性能提高最高，提高了8.92%。因此，这种参数组合被用于本文中的其他实验。此外，结果还表明，当w_{Pr}设置得较大（例如，w_{Pr}=1）而η设置得较小（例如，η=0.0）时，性能会下降。原因是过度考虑了车道的上游驶入流量（本质上是交叉口的未来状态），而忽略了交叉口的当前状态，导致性能下降。因此，平衡考虑交叉口的当前和未来状态对交通系统的性能至关重要。

---
<img src=Fig_15.jpg  width=70% />

**交叉口协同驾驶算法性能对比**. 我们将本文提出的基于MCTS的自适应算法与原始的基于MCTS的算法进行比较，以验证其性能优势。在相同的上层路由模型和交通需求下，我们分别部署了原始算法和自适应算法，并计算了相同路线上车辆的行驶时间。结果如上图所示。平均行驶时间结果（图15（a））表明，在我们的自适应协同驾驶算法下，车辆实现了更短的平均行驶时间。同时，随着到达率的增加，所提出的自适应算法的优点变得更加显著。图15（b）显示了行程时间的分布。结果表明，自适应算法将行驶时间的分布向左移动，特别避免了一些车辆行驶时间过长的问题。因此，研究结果表明，自适应协同驾驶算法通过考虑车道在空间和时间域中的优先级，在效率和公平性方面显著提高了全网流量内的协同驾驶性能。

---
<img src=Fig_16.jpg  width=95% />

**进一步研究自适应协同驾驶的效果**. 最后，我们使用一个特定的场景来进一步研究自适应车道优先级如何提高全网交通中的协同驾驶性能。我们用不同的协同驾驶算法求解同一场景的通过顺序，如上图所示。在这种情况下，南北车道上的车辆数量明显多于其他方向。原始的基于MCTS的算法没有考虑不同方向的排队和交通流量，只考虑控制区内车辆的实时状态信息。因此，在求解出的通行顺序中，南北车道上的车辆具有较低的优先级，而车辆较少的车道上的车辆具有较高的优先级。相反，本文提出的自适应协同驾驶算法求解出南北车道上车辆具有更高优先级的通过顺序。结果表明，自适应算法通过考虑更宽时空范围的车辆数量和驶入交通流量信息，自适应地提高了车辆较多车道的优先级，从而为相应车道上的车辆分配了更高的优先级。

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

