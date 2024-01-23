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

<img src=Fig1.jpg  width=95% />

**典型的群体机器人停车系统**. 典型的群体机器人停车常，车辆在停车场中不断进出。司机在停车场入口或下车区下车。停车场作业管理（POM）系统为其分配未占用的停车位，然后AGV机器人将车辆运输到分配的停车位中。通常，一个大型停车场包含数百个停车位，并根据布局划分为几个区域。为了增加单个训练结果的可扩展性，期望不同区域的拓扑结构相似。同时，为了充分发挥大型停车场的优势，到达的车辆通常均匀分布在不同的区域，或者根据驾驶员距离目的地的远近，根据就近原则进行区域分配。

---

<img src=Fig2.jpg  width=95% />

**我们提出的多AGV机器人泊车调度系统**. 系统分为任务调度、路线规划和轨迹规划。任务调度根据停车场的情况为到达的车辆分配停车位。给定地图和分配的停车位，路线规划通过避开静态障碍物来确定到达目的地的路线。轨迹规划计算纵向轨迹以遵循路线，同时避免碰撞和死锁。与上述三个子模块并行的另一个子模块是死锁检测和自愈模块，用于检测潜在的环形死锁并恢复锁定的机器人。

---
<img src=Fig3.jpg  width=90% />

**基于深度强化学习的任务调度模型之状态空间设置**

---

<img src=Fig4.jpg  width=90% />

**基于深度强化学习的任务调度模型**. 使用深度强化学习算法解决全局停车位分配问题主要有以下困难：（*i*）奖励是稀疏的，大多数随机选择的经验对模型学习的贡献很小；（*ii*） 即使在模拟环境中，对状态-动作空间的探索也是耗时的；（*iii*） 环境是动态的，许多随机因素（如车辆到达和离开时间的不确定性等）干扰模型训练，这使得事件奖励的方差很大。为了应对上述挑战，我们提出了一种基于原始深度Q网络（DQN）和现有改进技术的Double Dueling Deep Q-network。


---

<img src=Fig5.jpg  width=80% />

**基于深度强化学习的任务调度模型之深度网络设置**

---

<img src=Fig6.jpg  width=95% />

**多机器人冲突和死锁场景**。我们重点考虑冲突场景，其中容易发生拥塞和死锁。因此，轨迹规划模块在于求解存在冲突的群体AGV的安全高效轨迹，实现多辆AGV协同通过冲突区域。然而，多辆AGV的轨迹规划复杂而耗时，同时进行所有AGV的协同驾驶是不切实际的。因此，考虑到相距较远的AGV之间的弱相互作用，我们将封闭环境划分为一般局部区域，并将每个局部区域内的AGV轨迹规划为一组。通过上述场景分割，大大简化了多AGV协同驾驶的问题。上图显示了一个典型的局部场景。通常，在局部场景中有两种类型的冲突区域，即停车位前面的区域和十字路口。然而，与道路网络中的多交叉口不同，停车场内的冲突区域彼此靠近，因此车道经常出现交通拥堵。因此，为了减少等待时间并避免死锁，将协同规划即将穿越同一冲突区域的AGV的轨迹。特别的，上图中的*J*和*K*是死锁的，即它们等待彼此释放占用的空间。

---
<img src=Fig7.jpg  width=95% />

**典型冲突场景**.


---
<img src=Fig8.jpg  width=60% />

**基于规划的多机器人协同路权分配方法**. 我们采用基于树搜索的方法求解多机器人在冲突区域的路权协同方案，即通过冲突区域的优先级。根节点的子节点是所有可能的排列顺序。从第二层开始为每个附加层添加一个分离器，直到所有AGV分别通过冲突区域。但是，原始的树搜索方法没有考虑潜在的冲突和死锁。本文同时提出了修剪算法来删除不可行和不安全的方案，从而减少了轨迹规划的时间消耗。

---

<img src=Fig9.jpg  width=95% />

**两个或多个AGV之间不会因为争夺相同的空间资源而发生碰撞或死锁**. 在上层，基于DRL模型分配的停车区域。如果在指定的区域中没有可用的停车位，POM系统将在其他区域中随机分配停车位，以确保行驶到同一停车位的两辆AGV之间没有冲突。在较低级别中，首先检测任何可能的冲突区域。然后根据规划方法确定AGV通过冲突区的有效通过顺序。有效的通过顺序确保AGV不会因争夺交叉或重叠的空间资源而陷入碰撞或死锁。然而，由于AGV进出停车位的随机性，两个或多个冲突区域可能相邻或重叠。如上图所示，为了避免同一AGV在不同的局部合作场景中多次规划的矛盾，我们将重叠或相邻的冲突区域合并为统一场景。然后，在扩展的局部区域中进行协同轨迹规划。

---


<img src=Fig10.jpg  width=95% />

**多机器人死锁监测与自愈方法**.  与碰撞相比，死锁是群体机器人同时作业时常见的困难。上述基于规划的协同驾驶方式避免了冲突地区争夺空间的僵局。然而，由于每个AGV都沿着其最佳路径移动，因此存在多个AGV循环等待形式的潜在死锁。循环等待死锁是指一组AGV陷入无限等待中，以获得同一组中其他AGV所占用的空间。上图显示了循环等待死锁的一个示例。在环形等待中，当圆圈中的一个或多个AGV放弃任务或改变路径时，锁定的AGV可以恢复移动。据此，本文提出了相应的实时检测方法来检测循环等待死锁；在发生死锁时，通过重新分配停车位或为优先级较低的任务规划新路径来恢复该系统。

---

### *仿真实验*

<img src=Fig11.jpg  width=95% />

**虚拟实验场景**. 可以看到，拥堵主要是由AGV之间的冲突引起的，尤其是在路口等区域。

---

<img src=Fig12.jpg  width=40% />

<img src=Table3.jpg  width=60% />

**局部路权冲突场景下多机器人的协同**. 冲突区单元检测到A、B、C和D即将驶过交叉口区域，然后将它们作为一组进行协同轨迹规划。在生成并修剪解决方案树之后，剩下18个有效的通行顺序。分别计算了所有有效通行顺序的轨迹规划。结果显示，最优驾驶方案为*C|A|B|D*，耗时31.0s。显然，最优轨迹解决方案可以显著提高局部区域的运行效率，避免多辆AGV在路权冲突区域的碰撞和死锁。

---

<img src=Fig13.jpg  width=70% />

**底层协同轨迹规划的优越性**. 为了评估协同轨迹规划对整体交通拥堵缓解的效益，我们与不协同轨迹规划方法进行了比较实验，后者AGV采用先到先得的策略穿过冲突区域。作为性能指标，我们比较了150辆车进出停车场的平均时间消耗。上图显示了四种不同到达速率的结果。结果表明，无论到达率如何，协同轨迹规划方法都优于不协同轨迹规划方法。此外，随着平均到达率的增加，协同轨迹规划和不协同轨迹规划在时间消耗方面存在显著差异。


---

<img src=Fig16.jpg  width=70% />

**基于深度强化学习的机器人调度模型性能评估**. 为了分析所提出的基于DRL的方法的性能，我们开展了消融实验。上图显示了不同流量到达率下的评估结果。结果表明，基于DRL的分配方法可以显著节省大量时间。此外，将仿真结果与不同的观测特征进行比较，我们发现停车时长和取车地点是停车位分配的关键特征，而后者在大多数情况下起着更关键的作用。

---

<img src=Fig18.jpg  width=70% />

**基于深度强化学习的机器人调度模型的泛化性**. 上图显示了同一个模型在不同场景下的性能。结果显示，基于DRL的分配方法在各类场景下都具有更优的性能，这表明基于DRL方法对不断变化的环境具有很好的泛化性。

---

<img src=Fig14.jpg  width=70% />

**模型训练——不同奖励函数设置**. 

---

<img src=Fig15.jpg  width=70% />

**模型训练——不同周期设置**. 

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

