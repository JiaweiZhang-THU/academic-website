---
title: "BEV-V2X: Cooperative Birds-Eye-View Fusion and Grid Occupancy Prediction via V2X-Based Data Sharing"
authors:
- Cheng Chang
- admin
- Kunpeng Zhang
- Wenqin Zhong
- Xinyu Peng
- Shen Li
- Li Li
author_notes:
date: "2023-01-01T00:00:00Z"
doi: "10.1109/TIV.2023.3293954"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Intelligent Vehicles*"
publication_short: "IEEE T-IV"

abstract: Birds-Eye-View (BEV) perception can naturally represent natural scenes, which is conducive to multimodal data processing and fusion. BEV data contain rich semantics and integrate the information of driving scenes, which play an important role in researches related to autonomous driving. However, BEV constructed by single vehicle perception encounter certain issues, such as low accuracy and insufficient range, and thus cannot be well applied to scenario understanding and driving situation prediction. To address the challenges, this paper proposes a novel data-driven approach based on vehicle-to-everything (V2X) communication. The roadside unit or cloud center collects local BEV data from all connected and automated vehicles (CAVs) within the control area, then fuses and predicts the future global BEV occupancy grid map. It provides powerful support for driving safety warning, cooperative driving planning, cooperative traffic control and other applications. More precisely, we develop an attention-based cooperative BEV fusion and prediction model called BEV-V2X. We also compare the performance of BEV-V2X with that of single vehicle prediction. Experimental results demonstrate that our proposed method achieves higher accuracy. Even in cases where not all vehicles are CAVs, the model can still comprehensively estimate and predict global spatiotemporal changes. We also discuss the impact of the CAV rate, single vehicle perception ability, and grid size on the fusion and prediction results.

# Summary. An optional shortened abstract.
summary:  The roadside unit or cloud center collects local BEV data from all connected and automated vehicles (CAVs) within the control area, then fuses and predicts the future global BEV occupancy grid map. 

tags:
- Cooperative Driving
- Birds-Eye-View Fusion
- Occupancy Prediction
- BEV-V2X
featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/372296620_BEV-V2X_Cooperative_Birds-Eye-View_Fusion_and_Grid_Occupancy_Prediction_via_V2X-Based_Data_Sharing

url_pdf: https://ieeexplore.ieee.org/document/10179171/keywords#keywords
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

#### . An illustration of BEV perception based on single vehicle and CAV relative to vehicle A in an intersection scenario.
![avatar](./Fig_1.jpg)

---
#### The data flowchart of cooperative BEV fusion and prediction.
![avatar](./Fig_2.jpg)



---
#### The structure of spatial temporal attention.
![avatar](./Fig_4.jpg)


## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{10179171,
  author={Chang, Cheng and Zhang, Jiawei and Zhang, Kunpeng and Zhong, Wenqin and Peng, Xinyu and Li, Shen and Li, Li},
  journal={IEEE Transactions on Intelligent Vehicles}, 
  title={BEV-V2X: Cooperative Birds-Eye-View Fusion and Grid Occupancy Prediction via V2X-Based Data Sharing}, 
  year={2023},
  volume={},
  number={},
  pages={1-18},
  doi={10.1109/TIV.2023.3293954}
}
```

