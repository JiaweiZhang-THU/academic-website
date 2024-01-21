---
title: 训练调度模型的方法、装置、实现协同驾驶的方法及装置
subtitle: 已授权.


# Summary for listings and search engines
summary: 一种训练调度模型的方法、装置、实现协同驾驶的方法及装置.

# Link this post with a project
projects: []

# Date published
date: '2022-02-28T00:00:00Z'

# Date updated
lastmod: '2023-01-17T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - 李力
  - admin
  - 常成
  - 彭心宇

tags:
  - 专利

categories:
  - 文档
---


## 摘要
本文公开一种训练调度模型的方法、装置、实现协同驾驶的方法及装置,本发明实施例对样本车辆状态信息进行嵌入处理,映射出每一辆第一车辆相应的高维状态向量；对获得的高维状态向量进行处理,获得每一辆第一车辆相应的关联关系信息；根据获得的关联关系信息确定第一车辆的通行顺序信息；根据获得的通行顺序信息计算所有第一车辆通过无信号交叉口的延迟总和；根据计算出的延迟总和确定用于车辆调度的深度学习模型。本发明实施例通过离线的样本数据训练获得了可用于车辆调度的调度模型,通过调度模型缩短了车辆调度时长,提升了车辆调度的效率和质量。

## 主权项
一种训练调度模型的方法,包括：待训练的调度模型对输入的每一辆待通过无信号交叉口的第一车辆的样本车辆状态信息进行嵌入处理,获得各第一车辆相应的高维状态向量；其中,所述高维状态向量的维度为预设维度；对获得的高维状态向量进行处理,获得每一辆第一车辆的关联关系信息；其中,所述关联关系信息包括每一辆第一车辆的：高维状态向量和该第一车辆与其他第一车辆的冲突和耦合关系信息,其他第一车辆为该第一车辆自身以外的其他车辆；根据获得的关联关系信息确定第一车辆的通行顺序信息；根据获得的通行顺序信息计算所有待通过无信号交叉口的第一车辆均通过无信号交叉口的延迟总和；根据计算出的延迟总和确定待训练的调度模型的参数。

### [专利说明书](https://kns.cnki.net/kcms2/article/abstract?v=Epsgq4wCkk0Xh2jmtHk0yn5mIIDdkhxwlFDA37t5Dc00cKQiBYrOzqHi5iGxDKXT7xxU7qYMFhCn0SLPI3lx3Ok8fyMejP0X1lhSvuU9nloe2-yhEIfR1RB1uHI4XBbHwlnKTZFW7tI=&uniplatform=NZKPT&language=CHS)


