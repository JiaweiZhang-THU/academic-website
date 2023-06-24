---
title: "Coordinating CAV Swarms at Intersections with A Deep Learning Model"
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

abstract: Connected and automated vehicles (CAVs) have the potential to significantly improve the safety and efficiency of traffic. One revolutionary CAV’s impact on transportation system is cooperative driving that turns signalized intersections to be signal-free and boosts traffic efficiency by better organizing the passing order of CAVs. However, how to get the optimal passing order is an NP-hard problem (specifically, enumerating based algorithm takes days to find the optimal solution to a 20-CAV scenario). Here, we introduce a novel cooperative driving algorithm (AlphaOrder) that combines offline deep learning and online tree searching to find a near-optimal passing order in real-time. AlphaOrder builds a pointer network model from solved scenarios and generates near-optimal passing orders instantaneously for new scenarios. For the scenarios with 40 CAVs, AlphaOrder reduces the travel delay by more than 20% on average compared to the best-so-far MCTS based algorithm. Moreover, our algorithm provides a general approach to managing preemptive resource sharing between multi-agents (e.g., scheduling multiple automated guided vehicles (AGVs) and unmanned aerial vehicles (UAVs) at conflicting areas).

# Summary. An optional shortened abstract.
summary: AlphaOrder, a novel cooperative driving algorithm that combines offline deep learning and online tree searching to find a near-optimal passing order in real-time.


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

