---
title: "A Bi-level Network-wide Cooperative Driving Approach Including Deep Reinforcement Learning-based Routing"
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
publication: "*IEEE Transactions on Intelligent Vehicles*"
publication_short: "IEEE T-IV"

abstract: Cooperative driving of connected and automated vehicles (CAVs) has attracted extensive attention and researchers have proposed various approaches. However, existing approaches are limited to small-scale isolated scenarios and gaps remain in network-wide cooperative driving, especially in routing. In this paper, we decompose the network-level cooperative driving problem into two dominant sub-problems and accordingly propose a bi-level network-wide cooperative driving approach. The dynamic routing problem is considered in the upper level and we propose a multi-agent deep reinforcement learning (DRL) based routing model. The model can promote the equilibrium of network-wide traffic through distributed self-organized routing collaboration among vehicles, thereby improving efficiency for both individual vehicles and global traffic systems. In the lower level, we focus on the right-of-way assignment problem at signal-free intersections and propose an adaptive cooperative driving algorithm. The algorithm can adaptively evaluate priorities of different lanes, and then uses the lane priorities to guide the Monte Carlo tree search (MCTS) for better right-of-way assignments. Essentially, the upper level determines which conflict areas the vehicles will pass through, and the lower level addresses how the vehicles use the limited road resources more efficiently in each conflict area. The experimental results show that the upper and lower levels complement each other and work together to significantly improve the network-wide traffic efficiency and reduce the travel time of individual vehicles. Moreover, the results demonstrate that microscopic and mesoscopic cooperative driving behaviors of vehicles can significantly benefit the macroscopic traffic system.

# Summary. An optional shortened abstract.
summary: A novel bi-level network-wide cooperative driving approach for CAVs. (Upper) Multi-agent DRL based routing model. (Lower) Adaptive cooperative driving algorithm at intersections.


tags:
- Connected and Automated Vehicle
- Net-wide Traffic
- Cooperative Driving
- Signal-free Intersection
- Deep Reinforcement Learning
- Monte Carlo tree search
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

## The bi-level network-wide cooperative driving approach.
### An illustration of the proposed bi-level network-wide cooperative driving approach. In the upper level, the multi-agent deep reinforcement learning (DRL) based dynamic routing model takes the traffic state information from the macroscopic system as input and outputs the mesoscopic routing choices. In the lower level, the tree search based intersection cooperative driving algorithm takes the traffic state information from the mesoscopic system as input and outputs the microscopic passing order, i.e., the right-of-way assignment of vehicles passing through the conflict areas.
![avatar](./Fig_1.jpg)

---
### The overall framework of the bi-level network-wide cooperative driving approach for CAV swarms.
![avatar](./Fig_2.jpg)

---
## The dynamic routing problem formulation and corresponding reinforcement learning setup. 
#### （*a*） An illustration of the routing problem formulation. The red-shaded lanes are the candidate routes, and the blue-shaded lanes are the subsequent lanes corresponding to the two candidate routes. The traffic state information on the green-shaded area is the critical basis for dynamic routing decisions. The blue-dotted routes indicate the shortest subsequent routes for the candidate routes to the destination.
#### （*b*） Observation Space, where the left subfigure is one-step range observation and the right subfigure is two-step range observation. Furthermore, for ease of reading, it is necessary to illustrate the intersection markers. For example,*Node \# 1-2* refers to the second intersection that is one step away from the current node. And so on for the rest.

![avatar](./Fig_3.jpg)

---
## An illustration of the training pipeline of the upper-level multi-agent DRL based routing model. 
![avatar](./Fig_4.jpg)

---
## An illustration of the adaptive MCTS based cooperative driving algorithm.
#### (*left*) Queuing length information in the view zone (obtained by the roadside units at the current intersection) and drive-in traffic flow rate information of each lane (obtained by roadside units at the adjacent intersections and V2X communication) will be used to solve for the passing order of vehicles within the control zone (indicated by the blue dashed line).
#### (*right*) An illustration of the passing order. For example, "*BDEFCA*" is a feasible passing order. When the routes of two vehicles conflict, the more front the vehicle is in the passing order, the higher its priority is. For example, the priority of \emph{Vehicle D} is higher than the priority of *Vehicle A*.
![avatar](./Fig_5.jpg)

---
## The performance of AlphaOrder versus other algorithms on scenarios with different numbers of vehicles.
![avatar](./Fig_6.jpg)





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

