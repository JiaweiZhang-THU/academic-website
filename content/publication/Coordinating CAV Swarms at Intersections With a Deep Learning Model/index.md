---
title: "Coordinating CAV swarms at intersections with a deep learning model"
authors:
- admin
- Shen Li
- Li Li
author_notes:
date: "2023-06-01T00:00:00Z"
doi: "10.1109/TITS.2023.3250704"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-06-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.551)"
publication_short: "IEEE T-ITS"

abstract: 针对智能网联汽车协同决策问题面临的强交互资源受限、大规模*NP*难问题、强实时性约束等挑战，本研究提出基于深度模型的协同决策算法**AlphaOrder**。该算法通过结合离线深度学习模型和在线树搜索，实现了求解速度最快、效率最优的协同决策性能，比SOTA算法提高了55.6%。该研究为各类稀缺资源调度优化问题提供了通用的杰出算法。

# Summary. An optional shortened abstract.
summary: 当前性能最好的协同决策算法.


tags:
- 协同决策
- 智能网联汽车
- 协同驾驶
- 深度学习模型
- 无信号交叉口
- 深度强化学习
- 无监督学习
- Pointer神经网络
featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/369449074_Coordinating_CAV_Swarms_at_Intersections_With_a_Deep_Learning_Model
url_pdf: https://ieeexplore.ieee.org/abstract/document/10078727
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

**AlphaOrder算法的整体框架**。AlphaOrder以协同驾驶场景中的车辆状态信息作为输入，输出车辆通过路权冲突区域的通行顺序。AlphaOrder算法有两个核心的模块，其中Pointer神经网络用于快速端到端求解候选协同决策解，搜索树用于对协同决策解进行进一步优化。Critic神经网络作为基线来协助REINFORCE算法训练Pointer神经网络。此外，通过树搜索微调改进的解也可以用于进一步调优深度神经网络模型。

---

<img src=Fig_2.jpg  width=90% />

**Pointer网络和Critic网络的结构**. (*i*)Pointer网络：线性嵌入层首先嵌入由每辆车的速度、位置和意图（转向和路线）组成的状态信息。然后，将由车辆的嵌入信息组成的序列输入改进的编码器-解码器模型中，该模型由两个独立的LSTM神经网络单元组成。在每一步解码中，Pointer网络计算尚未被选择的车辆的条件概率，并选择概率最高的车辆（用红色箭头表示）加入通过顺序；（*ii*）Critic网络：Critic网络的嵌入层和编码器与Pointer网络具有相同的架构。通过多层全连接网络来计算编码信息，以输出目标函数值的预测。

---

<img src=Fig_3.jpg  width=90% />

**AlphaOrder算法中的分组和蒙特卡罗树搜索**。（*a*）分组：在深度模型输出的候选通过顺序中具有相邻位置的车辆被绑定到一组中。搜索树以组为基本单元（而不是车辆），能够有限缩小解空间，达到“短时微调”的目的。（*b*）蒙特卡洛书搜搜算法：（*i*）选择：根据最有希望的节点的得分选择节点；（*ii*）扩展：将尚未访问的子节点扩展到当前搜索树中；（*ii*）模拟：多轮次仿真模拟，直到达到一个叶节点，即获得完整的通过顺序；（*iv*）反向传播：根据叶节点的得分更新所有父节点的得分。

---
<img src=Fig_4.jpg  width=40% />

**实验场景**：一个典型的无信号交叉口，每个方向有三条车道。在实验中，我们将距离冲突区域*100m*的道路设置为控制区域，在协调路权时将考虑该范围内的车辆。

---
<img src=Fig_8.jpg  width=70% />

**AlphaOrder算法的最优性**。 为了展示AlphaOrder算法的最优性，我们详细研究了一个40辆车的问题实例。由于枚举所有的通行顺序是非常耗时的，我们花了大约50天的时间在其解决方案空间中统一枚举了大约6000万个可执行的通行顺序。即，我们在解空间上均匀采样了大约6000万个解。我们以直方图的方式对它们进行可视化。很明显，AlphaOrder在短时间内求解的传递顺序（深度模型耗时0.04s，随后的树搜索耗时0.1s）大致等于通过部分枚举找到的全局最优解，并且位于小概率的解空间中。同时，AlphaOrder明显优于基于FIFO和MCTS的算法，相应的性能提高了65.37%和55.55%。

---

<img src=Fig_9.jpg  width=70% />

**AlphaOrder算法的最优性**。 此外，为了评估AlphaOrder算法的平均性能，我们求解了车辆数目N=20、25、30、35、40时不同算法的性能。为了证明这两个模块在AlphaOrder中的关键作用，我们还绘制了Pointer网络产生的候选解。结果表明，对于包含任意数量车辆的场景，AlphaOrder算法可以找到目标函数更小的解，显著优于基于FIFO和MCTS的算法。对于有40辆车的场景，与迄今为止最好的基于MCTS的算法相比，AlphaOrder下的解的性能瓶颈提高了23.01%。结果还表明，Pointer网络可以直接为全新的场景生成有潜力的候选通过顺序，而短时树搜索可以进一步提高解的最优性。此外，我们可以看到，随着车辆数量的增加，基于MCTS的算法变得越来越不如我们的AlphaOrder算法，这正是由解空间的指数增长引起的。

---
<img src=Fig_10.jpg  width=70% />

**AlphaOrder算法的学习速度**。为了剖析AlphaOrder算法的学习速度，我们评估了Pointer网络在整个训练过程中的性能。上图显示了Pointer网络在训练和测试数据集上的性能，作为训练时期的函数。这里，训练数据集包含200000个问题实例；测试数据集包含1000个独立实例。结果表明，Pointer网络可以在一个Epoch后避免不可执行的解，即在看到一次训练实例后可以学习同一车道上车辆的前后约束。经过大约50个Epoch的探索，性能开始迅速提高。所有的网络都可以在150个Epoch内得到很好的训练（在一台机器上大约需要48小时）。结果还显示，在不超过75个Epoch后，Pointer网络产生的候选通过顺序开始优于基于MCTS的算法。此外，研究结果还表明，AlphaOrder的学习过程具有良好的稳定性。


---
<img src=Fig_11.jpg  width=70% />

**AlphaOrder算法的迁移性能**。预训练的模型可以有效地转移到新的场景，并且与从头开始训练的模型相比，预训练模型在短时间训练中实现了更好的性能。即使没有微调（对应于0Epoch），预训练的模型也可以为新的场景找到可执行的通行顺序，这表明不同交叉口之间潜在的经验共性。此外，预训练的模型只需3个Epoch（在单机上花费约20分钟）就可以大致达到最终性能。这有利于实际的大规模部署，即，给定预先训练的模型，我们可以通过短期迁移学习在不同的交叉口快速部署模型。

---

<img src=Fig_5.jpg  width=70% />

**AlphaOrder算法的性能**。AlphaOrder算法的最终性能对不同的数据集大小是鲁棒的，在训练速度和稳定性方面只有微小的差异。即使在一个小的训练数据集上，经过训练，AlphaOrder也能获得大致相同的性能，证明了AlphaOrder出色的学习能力。


---

<img src=Fig_6.jpg  width=70% />

**AlphaOrder算法的参数探讨**。

---

<img src=Fig_7.jpg  width=70% />

**AlphaOrder算法中的蒙特卡洛树搜索算法参数设置**。


---
**性能对比视频**

<img src="Problem_Instance_1_With_Vehicle_N=60.gif" alt="Example with 60 vehicles" style="zoom:100%;" />


---

## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10078727,
  author={Zhang, Jiawei and Li, Shen and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={Coordinating CAV Swarms at Intersections With a Deep Learning Model}, 
  year={2023},
  volume={24},
  number={6},
  pages={6280-6291},
  doi={10.1109/TITS.2023.3250704}
}
```



