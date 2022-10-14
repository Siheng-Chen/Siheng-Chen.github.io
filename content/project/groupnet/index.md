---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "GroupNet: Multiscale Hypergraph Neural Networks for Trajectory Prediction with Relational Reasoning"
summary: "**[ CVPR 2022 ]** <br>GroupNet, a multiscale hypergraph neural network, which is novel in terms of both interaction capturing and representation learning."
authors: [Chenxin Xu, Maosen Li, Zhenyang Ni, Ya Zhang, Siheng Chen]
tags: []
categories: [CVPR 2022]
date: 2022-04-18T19:34:19+08:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: Zhihu
  url: "TBD"
  icon_pack: fab
  icon: zhihu

url_code: "https://github.com/MediaBrain-SJTU/GroupNet"
url_pdf: "https://arxiv.org/abs/2204.08770"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

![](./images/featured.jpg)
## Abstract
Demystifying the interactions among multiple agents from their past trajectories is fundamental to precise and interpretable trajectory prediction. However, previous works only consider pair-wise interactions with limited relational reasoning. To promote more comprehensive interaction modeling for relational reasoning, we propose GroupNet, a multiscale hypergraph neural network, which is novel in terms of both interaction capturing and representation learning. From the aspect of interaction capturing, we propose a trainable multiscale hypergraph to capture both pair-wise and group-wise interactions at multiple group sizes. From the aspect of interaction representation learning, we propose a three-element format that can be learnt end-to-end and explicitly reason some relational factors including the interaction strength and category. We apply GroupNet into both CVAE-based prediction system and previous state-of-the-art prediction systems for predicting socially plausible trajectories with relational reasoning. To validate the ability of relational reasoning, we experiment with synthetic physics simulations to reflect the ability to capture group behaviors, reason interaction strength and interaction category. To validate the effectiveness of prediction, we conduct extensive experiments on three real-world trajectory prediction datasets, including NBA, SDD and ETH-UCY; and we show that with GroupNet, the CVAE-based prediction system outperforms state-of-the-art methods. We also show that adding GroupNet will further improve the performance of previous state-of-the-art prediction systems. 

## Result
### On the relational reasoning
Visualization of learnt group behavior. (a) The particle trajectories containing a three-group with a light bar, a two-group with a spring and an individual particle. (b) The heatmap of the learnt affinity matrix via affinity modeling. (c) The multiscale hypergraph topology via hyperedge forming and the interaction category vector of each hyperedge. The red box represents the three-group and two-group we inferred.
![](./images/group_behavior.png)

Particles' trajectories and the curve of neural interaction strength with particle's electric charge. We see that the neural interaction strength has a proportional relationship with the amount of charge, reflecting our model is capable to implicitly capture the interaction strength in an unsupervised manner. 
![](./images/strength.png)

Visualization results on the NBA dataset. We plot the best trajectory among 20 predictions for the state-of-the-art method (NMMP), GroupNet with the CVAE framework (Ours) and ground truth (GT). The red/blue color represents players of two teams and the green color represents the basketball. Light color represents the past trajectory.
![](./images/nba.png)

## Citation
```
@InProceedings{xu2022GroupNet,
author = {Xu, Chenxin and Li, Maosen and Ni, Zhenyang and Zhang, Ya and Chen, Siheng},
title = {GroupNet: Multiscale Hypergraph Neural Networks for Trajectory Prediction with Relational Reasoning},
booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
year = {2022}
}
```

## Acknowledgement
This research is partially supported by the National Key R&D Program of China under Grant 2021ZD0112801, National Natural Science Foundation of China under Grant 62171276, the Science and Technology Commission of Shanghai Municipal under Grant 21511100900 and CCF-DiDi GAIA Research Collaboration Plan 202112.
