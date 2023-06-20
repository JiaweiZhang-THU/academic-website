---
title: "A bi-level cooperative operation approach for AGV based automated valet parking"
authors:
- admin
- Zhiheng Li
- Li Li
- Yidong Li 
- Hairong Dong
author_notes:
date: "2021-04-01T00:00:00Z"
doi: ""

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
  preview_only: false

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

Conclusion: In this paper, a hierarchical cooperative operation approach is proposed to alleviate the traffic congestion problem of the AGV based AVP system. According to the leading causes of traffic congestion in the parking lot, we design a bi-level approach in which the upper-level considers the global parking space allocation, and the lower-level solves the cooperative driving problem of AGVs in the conflict zone. We innovatively formulate the parking space allocation problem into an MDP for the upper-level cooperation and then propose the Double Dueling DQN model to learn an outstanding allocation policy. For the lower-level cooperation, we divide the scenario according to the parking lot layout and then modify the planning based cooperative driving method to solve the safe and efficient trajectory of multiple AGVs in the conflict area. Meanwhile, the potential circle waits deadlock of multiple AGV is considered, and a real-time detection-and-recovery method is proposed. Finally, the effectiveness of the proposed approach is verified by numerical experiments, and the results show that the operation efficiency of the AGV based AVP system is significantly improved.↳

Future enhancements would be carried out in at least the following directions. First, the potential uncertainties should be integrated into the operation approach to improve the stability of the AVP system. Since there are some uncertainties in the environment of multiple AGVs, such as AGV broken during transportation, the operation approach can be dynamic and automatically handle the possible environment fluctuations. Second, future studies should consider the coordination among numerous computing units in distributed trajectory planning. As discussed in Section 7, distributed computing is inevitable due to the expansion of the parking scale. Therefore, further work needs to extend the centralized approach to distributed computing harmoniously. Finally, future work needs to reduce or even avoid the occurrence of potential circle deadlock. Based on the abstract acyclic priority graph, deadlock can be further reduced or completely avoided through top-level planning and reverse design of parking lot layout.

