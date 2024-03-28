---
title: "Drill the cork of information bottleneck by inputting the most important data"
authors:
- Xinyu Peng
- admin
- Fei-Yue Wang
- Li Li
author_notes:
date: "2022-10-28T00:00:00Z"
doi: "10.1109/TNNLS.2021.3079112"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-28T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*IEEE Transactions on Neural Networks and Learning Systems* <br /> (中科院1区; JCR Q1区; 影响因子=14.255)"
publication_short: "IEEE T-NNLS"

abstract: Deep learning has become the most powerful machine learning tool in the last decade. However, how to efficiently train deep neural networks remains to be thoroughly solved. The widely used minibatch stochastic gradient descent (SGD) still needs to be accelerated. As a promising tool to better understand the learning dynamic of minibatch SGD, the information bottleneck (IB) theory claims that the optimization process consists of an initial fitting phase and the following compression phase. Based on this principle, we further study typicality sampling, an efficient data selection method, and propose a new explanation of how it helps accelerate the training process of the deep networks. We show that the fitting phase depicted in the IB theory will be boosted with a high signal-to-noise ratio of gradient approximation if the typicality sampling is appropriately adopted. Furthermore, this finding also implies that the prior information of the training set is critical to the optimization process, and the better use of the most important data can help the information flow through the bottleneck faster. Both theoretical analysis and experimental results on synthetic and real-world datasets demonstrate our conclusions.

# Summary. An optional shortened abstract.
summary: We propose a new explanation of how typicality sampling helps accelerate the training process of the deep networks.


tags:
- Deep Learning
- Information Bottleneck
featured: false

# links:
# - name: ""
#   url: ""

links:
  - icon: researchgate
    icon_pack: fab
    name: Follow
    url: https://www.researchgate.net/publication/351834004_Drill_the_Cork_of_Information_Bottleneck_by_Inputting_the_Most_Important_Data
url_pdf: https://ieeexplore.ieee.org/abstract/document/9439803
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

 *下面为本研究的简介，详细内容请参阅[论文](https://ieeexplore.ieee.org/abstract/document/9439803)原文*

![avatar](./featured.jpg)

## Citation
If you find our work is useful in your research, please consider citing:
```
@ARTICLE{9439803,
  author={Peng, Xinyu and Zhang, Jiawei and Wang, Fei-Yue and Li, Li},
  journal={IEEE Transactions on Neural Networks and Learning Systems}, 
  title={Drill the Cork of Information Bottleneck by Inputting the Most Important Data}, 
  year={2022},
  volume={33},
  number={11},
  pages={6360-6372},
  doi={10.1109/TNNLS.2021.3079112}
}
```

