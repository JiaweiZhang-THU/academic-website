---
title: "A Bi-level Cooperative Operation Approach for AGV based Automated Valet Parking"
authors:
- admin
- Zhiheng Li
- Li Li
- Yidong Li 
- Hairong Dong
author_notes:
date: "2021-04-01T00:00:00Z"
doi: "10.1016/j.trc.2021.103140"

# Schedule page publish date (NOT publication's date).
publishDate: "2021-07-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*Transportation Research Part C: Emerging Technologies*"
publication_short: "TRC"

abstract: In urban areas, the number of cars has increased significantly in recent years, resulting in frequent traffic congestion in parking lots. Automated valet parking (AVP) system based on automated guided vehicles (AGVs) can relieve human from parking and improve efficiency to a certain extent due to their fully automatic control and operation. However, with the expansion of the scale of the whole parking lot, the current AGV based AVP system is facing the disadvantage of long-time queue congestion and even deadlock. In this paper, we systematically consider the traffic congestion faced by the AGV based AVP system and introduce a bi-level cooperative operation approach. The global cooperative parking space allocation is considered in the upper-level, and the cooperative driving of multiple AGVs in the conflict zone is resolved in the lower-level. The upper-level problem is formulated as a Markov decision process, and a global cooperative allocation method is obtained by using deep reinforcement learning (DRL). In the lower-level, with the modified planning based cooperative driving method, multiple AGVs can drive efficiently without collision and deadlock in the conflict zone. Experiment results show that the proposed cooperative operation approach can significantly alleviate the congestion problem in the AGV based parking lot and improve the AVP system’s efficiency.

# Summary. An optional shortened abstract.
summary: Deep reinforcement learning (DRL) based automated guided vehicles (AGVs) parking system.

tags:
- Source Themes
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
url_code: 'https://www.sciencedirect.com/science/article/pii/S0968090X21001583'
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
## AGV based Parking System
![avatar](./Fig1.jpg)

## Architecture
![avatar](./Fig2.jpg)

## DRL based Parking Space Allocation
#### The architecture of the DRL model for cooperative parking space allocation.
![avatar](./Fig4.jpg)

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

