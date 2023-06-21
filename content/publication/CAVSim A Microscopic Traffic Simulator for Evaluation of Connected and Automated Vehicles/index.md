---
title: "CAVSim: A microscopic traffic simulator for evaluation of connected and automated vehicles"
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
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-04-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Transportation Systems*"
publication_short: "IEEE T-ITS"

abstract: Connected and automated vehicles (CAVs) are expected to play a vital role in the emerging intelligent transportation system. In recent years, researchers have proposed various cooperative driving methods for CAVs, and there is an urgent need for a generic and unified traffic simulator to simulate and evaluate these methods. However, traditional traffic simulators have two critical deficiencies for CAV simulation needs, 1) the planning and dynamical modeling of vehicles in traditional simulators are based on a feedback mode, which is incompatible with the feed-forward decision and planning that CAVs commonly adopt; 2) the traditional simulators cannot provide typical traffic scenarios and corresponding standardized algorithms for multi-CAV cooperative driving. In this paper, we introduce CAVSim, a novel microscopic traffic simulator for CAVs, to address these deficiencies. CAVSim is developed modularly according to the emerging technology of the CAV environment, emphasizes feed-forward decision and planning for CAVs, and highlights the cooperative decision and planning components in the CAV environment. CAVSim incorporates rich and typical traffic scenarios and provides standardized cooperative driving algorithms and comparable performance metrics for multi-CAV cooperative driving. With CAVSim, researchers can conveniently deploy decision, planning, and control methods for CAVs at different levels, evaluate their performance, compare them with the standardized algorithms incorporated in CAVSim, and even further explore their impact on traffic flow. As a unified platform for CAVs, CAVSim can facilitate the studies on CAVs and promote the advancement of methods and techniques for CAVs.

# Summary. An optional shortened abstract.
summary: CAVSim, A traffic simulator for connected and automated vehicles (CAVs).

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
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
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

## The overall framework of CAVSim.
![avatar](./Fig_2.jpg)

---
## The bi-level framework of cooperative driving for CAV swarms. 
![avatar](./Fig_4.jpg)

---
##  A typical signal-free intersection. 
#### For example, “*BDEFCA*” is a feasible passing order. When the routes of two vehicles conflict, the more  front the vehicle is in the passing order, the higher its priority. For example, the priority of *Vehicle D* is higher than the priority of *Vehicle A*.

![avatar](./Fig_5.jpg)

---
##  A typical on-ramp merging scenario for connected and automated vehicles.
![avatar](./Fig_6.jpg)

---
## The velocities of a CAV platoon under different cruise settings in CAVSim.
#### We simulate the scenario that the speed of the leading vehicle (i.e., *Vehicle 1*) suddenly decelerates from *20m/s* to *5m/s* under different settings.
![avatar](./Fig_7.jpg)

---
##  Vehicle trajectories at the on-ramp scenario under different cooperative driving algorithms.
![avatar](./Fig_14.jpg)





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

