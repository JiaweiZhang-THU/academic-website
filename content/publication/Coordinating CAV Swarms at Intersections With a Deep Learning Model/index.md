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
publication: "*IEEE Transactions on Intelligent Transportation Systems*"
publication_short: "IEEE T-ITS"

abstract: 针对智能网联汽车协同决策问题面临的强交互资源受限、大规模*NP*难问题、强实时性约束等挑战，本研究提出基于深度模型的协同决策算法**AlphaOrder**。该算法通过结合离线深度学习模型和在线树搜索，实现了求解速度最快、效率最优的协同决策性能，比SOTA算法提高了55.6%。该研究为各类稀缺资源调度优化问题提供了通用的杰出算法。

# Summary. An optional shortened abstract.
summary: 当前性能最好的协同决策算法.


tags:
- Connected and Automated Vehicle
- Cooperative Driving
- Signal-free Intersection
- Deep Learning
- Deep Reinforcement Learning
- Pointer Network
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

## Training and online solving pipeline of AlphaOrder.
### AlphaOrder takes vehicles within the intersection scenario as the input, and its output is the passing order of these vehicles passing through the intersection.
![avatar](./Fig_1.jpg)

---
### Pointer and critic network architecture. 
![avatar](./Fig_2.jpg)

---
## Grouping and Monte Carlo tree search in AlphaOrder. 
#### （*a*） Grouping: Vehicles that have adjacent positions in candidate passing order are bound together into one group. The search tree grows with groups as the basic units (instead of vehicles). 
#### （*b*） MCTS algorithm: (*i*) Selection: selecting the most promising nodes based on their scores; (*ii*) Expansion: expanding the not-yet-visited child node into the current search tree; (*iii*) Simulation: running several rollout simulations until a leaf node is reached, i.e., a complete passing order is obtained; (*iv*) Backup: back-propagating to update the scores of all parent nodes based on the score of the leaf node.

![avatar](./Fig_3.jpg)

---
## A typical signal-free intersection with three lanes in each direction. 
#### In the experiments, we set the road with a length of *100m* from the conflict area as the control area (similarly hereinafter), and the vehicles within this range will be considered when coordinating the right-of-way. For safety reasons, vehicles in the control area are not allowed to change lanes.
![avatar](./Fig_4.jpg)

---
#### The histogram of delays of different passing orders for a problem instance with 40 vehicles.
![avatar](./Fig_8.jpg)

---
####  The performance of AlphaOrder versus other algorithms on scenarios with different numbers of vehicles.
![avatar](./Fig_9.jpg)





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

