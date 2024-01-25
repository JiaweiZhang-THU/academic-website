---
title: "Predictive information multiagent deep reinforcement learning for automated truck platooning control"
authors:
- Renzong Lian
- Zhiheng Li
- Boxuan Wen
- Junqing Wei
- admin
- Li Li
author_notes:
date: "2022-10-01T00:00:00Z"
doi: "10.1109/MITS.2023.3319091"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Intelligent Transportation Systems Magazine*"
publication_short: "MITS"

abstract: Human-leading automated truck platooning has been an effective technique to improve traffic capacity and fuel economy and eliminate uncertainties of the traffic environment. Aiming for a tradeoff between the dynamic response of car following and energy-efficient platooning control, a predictive information multiagent soft actor–critic (PI-MASAC) control framework is proposed for a human-leading automated heavy-duty-truck platoon. In this framework, predictive information of environmental dynamics is modeled as the state representation of a deep reinforcement learning algorithm to address the uncertainties of a partially observable environment. In the truck model, the impact of intraplatoon aerodynamic interactions is modeled, which is used to design a constant spacing policy for platooning control. We demonstrate the effectiveness of our approach by testing the human-leading truck platoon under multiple scenarios compared to proximal policy optimization, an intelligent driver model, and linear-based cooperative adaptive cruise control. Our results show that the PI-MASAC learns a novel car-following strategy of peak shaving and valley filling and therefore significantly enhances energy savings by reducing high-intensity accelerations and decelerations. In addition, the PI-MASAC demonstrates its adaptability to various initial scenarios and exhibits good generalization to a larger platoon size.

# Summary. An optional shortened abstract.
summary: A predictive information multiagent soft actor–critic (PI-MASAC) control framework is proposed for a human-leading automated heavy-duty-truck platoon.


tags:
- Autonomous vehicles 
- automated truck platooning
- Vehicle dynamics 
- Estimation 
- Stability analysis 
featured: false

# links:
# - name: ""
#   url: ""
links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/374527166_Multiagent_Deep_Reinforcement_Learning_for_Automated_Truck_Platooning_Control
url_pdf: https://ieeexplore.ieee.org/abstract/document/10273625
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

 *详细内容请参阅[论文](https://ieeexplore.ieee.org/abstract/document/10273625)原文*


<img src=featured.jpg  width=90% />

## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10273625,
  author={Lian, Renzong and Li, Zhiheng and Wen, Boxuan and Wei, Junqing and Zhang, Jiawei and Li, Li},
  journal={IEEE Intelligent Transportation Systems Magazine}, 
  title={Multiagent Deep Reinforcement Learning for Automated Truck Platooning Control}, 
  year={2023},
  volume={},
  number={},
  pages={2-17},
  doi={10.1109/MITS.2023.3319091}}
```

