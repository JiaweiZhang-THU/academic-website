---
title: "Multi-agent DRL-based lane change with right-of-way collaboration awareness"
authors:
- admin
- Cheng Chang
- Xianlin Zeng
- Li Li
author_notes:
- [scholar](https://scholar.google.com/citations?user=I_7YQWsAAAAJ&hl=zh-CN&authuser=1)
- [scholar](https://scholar.google.com/citations?user=NNWr5EwAAAAJ&hl=zh-CN&authuser=1)
date: "2022-10-28T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems*"
publication_short: "IEEE T-ITS"

abstract: Lane change is a common-yet-challenging driving behavior for automated vehicles. To improve the safety and efficiency of automated vehicles, researchers have proposed various lane-change decision models. However, most of the existing models consider lane-change behavior as a one-player decision-making problem, ignoring the essential multi-agent properties when vehicles are driving in traffic. Such models lead to deficiencies in interaction and collaboration between vehicles, which results in hazardous driving behaviors and overall traffic inefficiency. In this paper, we revisit the lane-change problem and propose a bi-level lane-change behavior planning strategy, where the upper level is a novel multi-agent deep reinforcement learning (DRL) based lane-change decision model and the lower level is a negotiation based right-of-way assignment model. We promote the collaboration performance of the upper-level lane-change decision model from three crucial aspects. First, we formulate the lane-change decision problem with a novel multi-agent reinforcement learning model, which provides a more appropriate paradigm for collaboration than the single-agent model. Second, we encode the driving intentions of surrounding vehicles into the observation space, which can empower multiple vehicles to implicitly negotiate the right-of-way in decision-making and enable the model to determine the right-of-way in a collaborative manner. Third, an ingenious reward function is designed to allow the vehicles to consider not only ego benefits but also the impact of changing lanes on traffic, which will guide the multi-agent system to learn excellent coordination performance. With the upper-level lane-change decisions, the lower-level right-of-way assignment model is used to guarantee the safety of lane-change behaviors. The experiments show that the proposed approaches can lead to safe, efficient, and harmonious lane-change behaviors, which boosts the collaboration between vehicles and in turn improves the safety and efficiency of the overall traffic. Moreover, the proposed approaches promote the microscopic synchronization of vehicles, which can lead to the macroscopic synchronization of traffic flow.

# Summary. An optional shortened abstract.
summary: A novel multi-agent deep reinforcement learning (DRL) based lane-change decision model.

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: https://ieeexplore.ieee.org/abstract/document/9932003
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
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
## The overall architecture of the proposed bi-level lane-change behavior planning strategy.
![avatar](./featured.jpg)

## An illustration of the traffic snapshot and driving intention.
![avatar](./Fig_2.jpg)

## The training pipeline of the upper-level SAC based lane-change decision model.
![avatar](./Fig_3.jpg)



# Performance

#### Average speed of traffic flow under different lane-change decision models. The baseline denotes that lane changes are not allowed and all vehicles keep the lanes.
![avatar](./Fig_4.jpg)


#### Screenshot of the traffic simulation, where we enable only the upper-level lane-change decision model but do not enable the lower-level right-ofway assignment model. *Vehicle A* and *Vehicle B* collide during executing the lane-change actions.
![avatar](./Fig_11.jpg)


#### Screenshot of traffic simulation with the proposed bi-level lanechange behavior planning strategy. The lower-level right-of-way assignment model avoids the potential collision between *Vehicle C* and *Vehicle D*.
![avatar](./Fig_12.jpg)


#### Vehicle trajectories in congested traffic with different lane-change decision models. The upper subfigure is from the model that only considers ego benefits, and the lower subfigure is from the proposed model.
![avatar](./Fig_14.jpg)





## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{9932003,
  author={Zhang, Jiawei and Chang, Cheng and Zeng, Xianlin and Li, Li},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={Multi-Agent DRL-Based Lane Change With Right-of-Way Collaboration Awareness}, 
  year={2023},
  volume={24},
  number={1},
  pages={854-869},
  doi={10.1109/TITS.2022.3216288}
}
```

