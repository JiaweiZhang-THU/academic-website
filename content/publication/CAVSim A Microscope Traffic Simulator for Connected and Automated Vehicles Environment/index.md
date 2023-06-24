---
title: "CAVSim: A Microscope Traffic Simulator for Connected and Automated Vehicles Environment"
authors:
- admin
- Cheng Chang
- Huaxin Pei
- Xinyu Peng
- Yuqing Guo
- Renzong Lian
- ZhenwuChen
- Li Li
author_notes:
date: "2022-10-08T00:00:00Z"
doi: "10.1109/ITSC55140.2022.9922267"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-08T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*2022 IEEE 25th International Conference on Intelligent Transportation Systems (ITSC)*"
publication_short: "IEEE ITSC"

abstract: Connected and automated vehicles (CAVs) are expected to play a vital role in the next-generation intelligent transportation system. In recent years, researchers have proposed various cooperative driving methods for CAVs' decisions and planning, and there is an urgent need for a suitable and unified traffic simulator to evaluate and test these methods. However, existing traffic simulators have three critical deficiencies for CAV simulation needs, (1) most of them are from the perspective of traffic flow simulation and have strong simplification and assumptions for vehicle modeling; (2) CAVs are different from traditional human-driven vehicles (HVs) and have new properties, which require new driving models; (3) the existing traffic simulators are inconvenient to deploy the emerging cooperative driving methods because their modeling of the traffic system architecture is traditional. In this paper, we introduce CAVSim, a novel microscope traffic simulator for the CAV environment, to address these deficiencies. CAVSim is modularly developed according to the emerging architecture for the CAV environment, emphasizes more detailed driving behaviors of CAVs, and highlights the decision and planning components in the CAV environment. With CAVSim, researchers can quickly deploy decision and planning methods at different levels, evaluate and test their performance, and explore their impact on the traffic flow in the CAV environment.

# Summary. An optional shortened abstract.
summary: CAVSim, A traffic simulator for connected and automated vehicles (CAVs).

tags: 


# Display this page in the Featured widget?
featured: true

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/364997777_CAVSim_A_Microscope_Traffic_Simulator_for_Connected_and_Automated_Vehicles_Environment
url_pdf: https://ieeexplore.ieee.org/abstract/document/9922267
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

## CAVSim A Microscope Traffic Simulator for Connected and Automated Vehicles Environment.
![avatar](./Fig1.jpg)

---
## The overall framework of the CAVSim simulator.
![avatar](./Fig2.jpg)

---
##  Vehicle trajectories at signal-free intersection under different cooperative driving methods.
#### (a) Vehicle trajectories under FIFO based cooperative driving. (b) Vehicle trajectories under MCTS based cooperative driving.

![avatar](./Fig5.jpg)




## Citation
If you find our work is useful in your research, please consider citing:
```
@INPROCEEDINGS{9922267,
  author={Zhang, Jiawei and Chang, Cheng and Pei, Huaxin and Peng, Xinyu and Guo, Yuqing and Lian, Renzong and Chen, Zhenwu and Li, Li},
  booktitle={2022 IEEE 25th International Conference on Intelligent Transportation Systems (ITSC)}, 
  title={CAVSim: A Microscope Traffic Simulator for Connected and Automated Vehicles Environment}, 
  year={2022},
  volume={},
  number={},
  pages={3719-3724},
  doi={10.1109/ITSC55140.2022.9922267}
}

```

