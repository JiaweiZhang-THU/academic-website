---
title: "CAVSim: a microscopic traffic simulator for evaluation of connected and automated vehicles"
authors:
- admin
- Cheng Chang
- Zimin He
- Wenqin Zhong
- Danya Yao
- Shen Li
- Li Li
author_notes:
date: "2023-04-24T00:00:00Z"
doi: "10.1109/TITS.2023.3273565"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-04-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems* <br /> (中科院1区TOP期刊; JCR Q1区; 影响因子=9.551)"
publication_short: "IEEE T-ITS"

abstract: 针对自动驾驶仿真在前馈式决策规划、多车协同决策、基准场景算法、测试验证评估等方面的迫切需求，本工作研发了自动驾驶仿真测试平台CAVSim。该平台能够满足以上仿真需求，突出自动驾驶前馈式决策与规划，支持多车协同驾驶仿真。同时，该平台嵌入了丰富的协同决策场景、基准算法、测试功能，具有重要的研究和应用价值。该平台在开源后得到广泛应用，已有数十篇高水平学术论文基于该平台发表.

# Summary. An optional shortened abstract.
summary: 面向高级别自动驾驶技术的自动驾驶仿真平台.

tags:
- 自动驾驶仿真
- 自动驾驶测试
- 自动驾驶汽车
- 智能网联汽车
- 决策规划
- 微观交通仿真
- 车队稳定性测试


featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/370731657_CAVSim_A_Microscopic_Traffic_Simulator_for_Evaluation_of_Connected_and_Automated_Vehicles
url_pdf: https://ieeexplore.ieee.org/abstract/document/10124078
url_code: 'https://github.com/JiaweiZhang-THU/CAVSim'
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
  - Connected and Automated Vehicles Simulation Platform

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---



 *下面为本研究的简要介绍，详细内容请参阅[论文](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10221733)原文*


<img src=Fig_1.jpg  width=50% />

**典型的智能网联汽车和自动驾驶汽车仿真环境**

---

<img src=Fig_2.jpg  width=95% />

**CAVSim的核心架构**. 基于模块化原理，设计了CAVSim的总体框架。CAVSim有三个核心组件：对象、算法和测试相关。首先，对象模块的元素，即道路和车辆，是用于构建仿真环境的主要组件，它们将频繁交互以模拟智能网联环境。其次，算法模块提供了有关交通和车辆的决策和规划方法。同时，算法模块专门提供各种接口，使研究人员可以通过改变某个接口来部署不同的算法，然后在CAVSim上进行微观自动驾驶仿真，以模拟和评估他们的方法。第三，测试相关模块提供了典型的标准化算法和可比较的性能指标。此外，紫色模块中的车辆更新流程图总结了CAVSim中车辆驾驶感知-决策-行动循环的主要步骤。

---

<img src=Fig_3.jpg  width=50% />

**对象模块——道路**. 道路是微观交通仿真环境的主要组成部分。在智能网联环境中，路测设备赋予道路丰富的角色和功能。为了增加CAVSim中交通场景的可扩展性，并考虑略侧设备的边缘性，我们基于典型的交通场景对道路进行分段，以获得基本的道路块，如图所示。3。

---

<img src=Fig_4.jpg  width=50% />

**前馈式决策规划示例**。在CAVSim中，自动驾驶车辆群体通过无信号交叉口的问题采用双层框架解决。在上层，集中式算法将冲突区域的通行权分配给控制区域中的车辆，而在下层，分布式轨迹规划算法基于集中式算法的输出以前馈模式规划车辆的运动。


---

<img src=Fig_5.jpg  width=50% />

**典型的无信号交叉口**。例如，“*BDEFCA*”是一个可行的通行顺序。当两辆车的路线冲突时，车辆在通过顺序中越靠前，其优先级就越高。例如，车辆*D*的优先级高于车辆*A*的优先级。

---
<img src=Fig_6.jpg  width=50% />

**典型的匝道合流区域**。自动驾驶车辆群体在匝道处合流是另一种典型的关键交通场景，其中智能网联技术将显著提高合流的安全性和效率。与无信号交叉口类似，匝道上的协同驾驶通常由双层框架解决。上层集中式算法解决了车辆的优先级关系，也可以称为通过顺序。下层分布式算法求解最优轨迹。

---
<img src=Fig_7.jpg  width=50% />

**实验场景**：一个典型的无信号交叉口，每个方向有三条车道。在实验中，我们将距离冲突区域*100m*的道路设置为控制区域，在协调路权时将考虑该范围内的车辆。




## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10124078,
  author={Zhang, Jiawei and Chang, Cheng and He, Zimin and Zhong, Wenqin and Yao, Danya and Li, Shen and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={CAVSim: A Microscopic Traffic Simulator for Evaluation of Connected and Automated Vehicles}, 
  year={2023},
  volume={},
  number={},
  pages={1-17},
  doi={10.1109/TITS.2023.3273565}
}
```

