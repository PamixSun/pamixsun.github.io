---
layout: post
title:  "Optic Disc and Cup Localization from Retinal Fundus Images via Deep Object Detection Networks"
date:   2018-3-31
categories: update
---

### Background

Glaucoma, as the second leading cause of blindness worldwide, is predicted to affect approximately 80 million people by 2020. As damage to the optic nerve is irreversible, early detection of glaucoma is critical to prevent further vision deterioration. The cup-to-disc ratio (CDR) is commonly used for glaucoma diagnosis. Therefore, accurate segmentation of the optic disc (OD) and optic cup (OC) is essential for automated glaucoma screening. 

### Object Detection based Method

![plot of chunk image_1](/images/deepCDR/framework.jpg)

In this paper, we formulate the optic disc/optic cup segmentation as a multi-object detection problem, with the introduction of objectness constraints to improve accuracy. Unlike traditional pixel-wise two-step approaches, we propose a simple yet effective one-step method to jointly localize and segment the optic disc and optic cup in retinal fundus images using deep object detection networks. The proposed method inherently has four advantages: 1) The multi-object detection network incorporates the relationship between optic disc and optic cup and localizes them simultaneously; 2) The object detection network contains objectness properties, providing high-level object constraints; 3) The end-to-end architecture enables automatic learning of image features, and also allows for transfer learning to address the challenge of small-scale data; 4) Our deep object detection based method is not only conceptually simpler but also easier to deploy compared to other multi-step methods such as M-Net. Evaluated on the widely used public ORIGA dataset, our method outperforms all existing methods, achieving state-of-the-art segmentation performance. Moreover, the proposed method obtains satisfactory glaucoma screening performance with cup-to-disc ratio calculated on the ORIGA and SCES datasets.

### Papers

This work has been accepted by **the IEEE International Symposium on Biomedical Imaging (ISBI) 2018** as a one-page abstract.



