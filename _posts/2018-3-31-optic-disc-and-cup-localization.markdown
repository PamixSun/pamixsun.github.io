---
layout: post
title:  "Optic Disc and Cup Localization from Retinal Fundus Images via Deep Object Detection Networks"
date:   2018-3-31
categories: update
---

### Background

As the second leading cause of blindness, glaucoma is predicted to affect about 80 million people by 2020. Since damage to optic nerves cannot be reversed, early detection of glaucoma is critical in preventing further deterioration. The cup-to-disc ratio (CDR) is commonly used for glaucoma diagnosis. Thus, accurate segmentation of optic disc (OD) and optic cup (OC) is essential for automated glaucoma screening.

### Object Detection based Method

![plot of chunk image_1](/images/deepCDR/framework.jpg)

In this paper, we introduce athe objectness constrain in to the OD/OC segmentation problem, and gain the higher level discriminate representation based on the deep object detection system. Different from traditional pixel-wise based two-step approaches, we propose a simple yet effective one-step method to jointly localizae/segment OD and OC in a retinal fundus image based on deep object detection networks. THe proposed method inherently holds four desirable features: 1) the multi-object network involves the OD and OC relationship and localizes them simultaneously; 2) the object detection network contains the objectness property, which presents the high level object constrain; 3) the end-to-end architecture guarantees learning image features automatically, and also allows for transfer learning to address the challenging of small scale data; 4) our deep object detection based method is not only conceptually simpler but also easier to deploy comparing to other multi-step methods such as M-Net. Evaluated on the widely and publicly available ORIGA dataset, our method outperforms all existing methods, achieving state-of-the-art segmentation performance, Moreover, the proposed method also obtains satisfactory glaucoma screening performance with CDR calculated on the ORIGA and SCES datasets.




