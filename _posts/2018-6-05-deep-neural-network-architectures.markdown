---
layout: post
title:  "Deep Neural Network Architectures: A Reading List"
date:   2018-6-05
categories: update
---

### Image Recognition

**AlexNet**:

Krizhevsky, Alex, Ilya Sutskever, and Geoffrey E. Hinton. "Imagenet classification with deep convolutional neural networks." In Advances in neural information processing systems, pp. 1097-1105. 2012.

**NiN**:

Lin, Min, Qiang Chen, and Shuicheng Yan. "Network in network." arXiv preprint arXiv:1312.4400 (2013).

**ZFNet**:

Zeiler, Matthew D., and Rob Fergus. "Visualizing and understanding convolutional networks." In European conference on computer vision, pp. 818-833. Springer, Cham, 2014.

**VGGNet**:

Simonyan, Karen, and Andrew Zisserman. "Very deep convolutional networks for large-scale image recognition." arXiv preprint arXiv:1409.1556 (2014).

**GoogLeNet (Inception)**:

Szegedy, Christian, Wei Liu, Yangqing Jia, Pierre Sermanet, Scott Reed, Dragomir Anguelov, Dumitru Erhan, Vincent Vanhoucke, and Andrew Rabinovich. "Going deeper with convolutions." CVPR, 2015.

Ioffe, Sergey, and Christian Szegedy. "Batch normalization: Accelerating deep network training by reducing internal covariate shift." arXiv preprint arXiv:1502.03167 (2015).

Szegedy, Christian, Vincent Vanhoucke, Sergey Ioffe, Jon Shlens, and Zbigniew Wojna. "Rethinking the inception architecture for computer vision." In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition, pp. 2818-2826. 2016.

Szegedy, Christian, Sergey Ioffe, Vincent Vanhoucke, and Alexander A. Alemi. "Inception-v4, inception-resnet and the impact of residual connections on learning." In AAAI, vol. 4, p. 12. 2017.

**Xception**:

Chollet, François. "Xception: Deep learning with depthwise separable convolutions." arXiv preprint (2016).

**ResNet**:

He, Kaiming, Xiangyu Zhang, Shaoqing Ren, and Jian Sun. "Deep residual learning for image recognition." In Proceedings of the IEEE conference on computer vision and pattern recognition, pp. 770-778. 2016.

**ResNeXT**:

Xie, Saining, Ross Girshick, Piotr Dollár, Zhuowen Tu, and Kaiming He. "Aggregated residual transformations for deep neural networks." In Computer Vision and Pattern Recognition (CVPR), 2017 IEEE Conference on, pp. 5987-5995. IEEE, 2017.

**DenseNet**:

Huang, Gao, Zhuang Liu, Kilian Q. Weinberger, and Laurens van der Maaten. "Densely connected convolutional networks." In Proceedings of the IEEE conference on computer vision and pattern recognition, vol. 1, no. 2, p. 3. 2017.

**SqueezeNet**:

Iandola, Forrest N., Song Han, Matthew W. Moskewicz, Khalid Ashraf, William J. Dally, and Kurt Keutzer. "SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and< 0.5 MB model size." arXiv preprint arXiv:1602.07360 (2016).

**SENet**:

Hu, Jie, Li Shen, and Gang Sun. "Squeeze-and-excitation networks." arXiv preprint arXiv:1709.01507 (2017).

**MobileNet**:

Howard, Andrew G., Menglong Zhu, Bo Chen, Dmitry Kalenichenko, Weijun Wang, Tobias Weyand, Marco Andreetto, and Hartwig Adam. "Mobilenets: Efficient convolutional neural networks for mobile vision applications." arXiv preprint arXiv:1704.04861 (2017).

Sandler, Mark, Andrew Howard, Menglong Zhu, Andrey Zhmoginov, and Liang-Chieh Chen. "MobileNetV2: Inverted Residuals and Linear Bottlenecks." arXiv preprint arXiv:1801.04381 (2018).

**ShuffleNet**:

Zhang, Xiangyu, Xinyu Zhou, Mengxiao Lin, and Jian Sun. "Shufflenet: An extremely efficient convolutional neural network for mobile devices." arXiv preprint arXiv:1707.01083 (2017).

**Dual path Nets**:

Chen, Yunpeng, Jianan Li, Huaxin Xiao, Xiaojie Jin, Shuicheng Yan, and Jiashi Feng. "Dual path networks." In Advances in Neural Information Processing Systems, pp. 4470-4478. 2017.

### Object Detection

#### Two Stage Methods:

**R-CNN**:

Girshick, Ross, Jeff Donahue, Trevor Darrell, and Jitendra Malik. "Region-based convolutional networks for accurate object detection and segmentation." IEEE transactions on pattern analysis and machine intelligence 38, no. 1 (2016): 142-158.

**SPP-Net**:

He, Kaiming, Xiangyu Zhang, Shaoqing Ren, and Jian Sun. "Spatial pyramid pooling in deep convolutional networks for visual recognition." IEEE transactions on pattern analysis and machine intelligence 37, no. 9 (2015): 1904-1916.

**Fast R-CNN**:

Girshick, Ross. "Fast R-CNN." In Computer Vision (ICCV), 2015 IEEE International Conference on, pp. 1440-1448. IEEE, 2015.

**Faster R-CNN**:

Ren, Shaoqing, Kaiming He, Ross Girshick, and Jian Sun. "Faster r-cnn: Towards real-time object detection with region proposal networks." In Advances in neural information processing systems, pp. 91-99. 2015.

**MR-CNN**:

Gidaris, Spyros, and Nikos Komodakis. "Object detection via a multi-region and semantic segmentation-aware cnn model." In Proceedings of the IEEE International Conference on Computer Vision, pp. 1134-1142. 2015.

**HyperNet**:

Kong, Tao, Anbang Yao, Yurong Chen, and Fuchun Sun. "Hypernet: Towards accurate region proposal generation and joint object detection." In Proceedings of the IEEE conference on computer vision and pattern recognition, pp. 845-853. 2016.

**CRAFT**:

Yang, Bin, Junjie Yan, Zhen Lei, and Stan Z. Li. "CRAFT Objects from Images." In Computer Vision and Pattern Recognition (CVPR), 2016 IEEE Conference on, pp. 6043-6051. IEEE, 2016.

**R-FCN**:

Dai, Jifeng, Yi Li, Kaiming He, and Jian Sun. "R-fcn: Object detection via region-based fully convolutional networks." In Advances in neural information processing systems, pp. 379-387. 2016.

**MS-CNN**:

Cai, Zhaowei, Quanfu Fan, Rogerio S. Feris, and Nuno Vasconcelos. "A unified multi-scale deep convolutional neural network for fast object detection." In European Conference on Computer Vision, pp. 354-370. Springer, Cham, 2016.

**PVANet**:

Hong, Sanghoon, Byungseok Roh, Kye-Hyeon Kim, Yeongjae Cheon, and Minje Park. "PVANet: Lightweight Deep Neural Networks for Real-time Object Detection." arXiv preprint arXiv:1611.08588 (2016).

**FPN**:

Lin, Tsung-Yi, Piotr Dollár, Ross Girshick, Kaiming He, Bharath Hariharan, and Serge Belongie. "Feature pyramid networks for object detection." In CVPR, vol. 1, no. 2, p. 4. 2017.

**Mask R-CNN**:

He, Kaiming, Georgia Gkioxari, Piotr Dollár, and Ross Girshick. "Mask r-cnn." In Computer Vision (ICCV), 2017 IEEE International Conference on, pp. 2980-2988. IEEE, 2017.

**A-Fast-RCNN**:

Wang, Xiaolong, Abhinav Shrivastava, and Abhinav Gupta. "A-Fast-RCNN: Hard Positive Generation via Adversary for Object Detection." In Computer Vision and Pattern Recognition (CVPR), 2017 IEEE Conference on, pp. 3039-3048. IEEE, 2017.

**CoupleNet**:

Zhu, Yousong, Chaoyang Zhao, Jinqiao Wang, Xu Zhao, Yi Wu, and Hanqing Lu. "Couplenet: Coupling global structure with local parts for object detection." In Proc. of Int’l Conf. on Computer Vision (ICCV). 2017.

**MegDet**:

Peng, Chao, Tete Xiao, Zeming Li, Yuning Jiang, Xiangyu Zhang, Kai Jia, Gang Yu, and Jian Sun. "MegDet: A Large Mini-Batch Object Detector." arXiv preprint arXiv:1711.07240 (2017).

**Light-Head R-CNN**:

Li, Zeming, Chao Peng, Gang Yu, Xiangyu Zhang, Yangdong Deng, and Jian Sun. "Light-Head R-CNN: In Defense of Two-Stage Object Detector." arXiv preprint arXiv:1711.07264 (2017).

#### One Stage Methods:

**OverFeat**:

Sermanet, Pierre, David Eigen, Xiang Zhang, Micha毛l Mathieu, Robert Fergus, and Yann Lecun. "Overfeat: Integrated recognition, localization and detection using convolutional networks." In聽International Conference on Learning Representations (ICLR2014), CBLS, April 2014. 2014.

**YOLO**:

Redmon, Joseph, Santosh Divvala, Ross Girshick, and Ali Farhadi. "You only look once: Unified, real-time object detection." In Proceedings of the IEEE conference on computer vision and pattern recognition, pp. 779-788. 2016.

**YOLOv2 & YOLO9000**:

Redmon, Joseph, and Ali Farhadi. "YOLO9000: Better, Faster, Stronger." In Computer Vision and Pattern Recognition (CVPR), 2017 IEEE Conference on, pp. 6517-6525. IEEE, 2017.

**G-CNN**:

Najibi, Mahyar, Mohammad Rastegari, and Larry S. Davis. "G-cnn: an iterative grid based object detector." In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition, pp. 2369-2377. 2016.

**SSD**:

Liu, Wei, Dragomir Anguelov, Dumitru Erhan, Christian Szegedy, Scott Reed, Cheng-Yang Fu, and Alexander C. Berg. "Ssd: Single shot multibox detector." In European conference on computer vision, pp. 21-37. Springer, Cham, 2016.

**R-SSD**:

Jeong, Jisoo, Hyojin Park, and Nojun Kwak. "Enhancement of SSD by concatenating feature maps for object detection." arXiv preprint arXiv:1705.09587 (2017).

**DSSD**:

Fu, Cheng-Yang, Wei Liu, Ananth Ranga, Ambrish Tyagi, and Alexander C. Berg. "DSSD: Deconvolutional single shot detector." arXiv preprint arXiv:1701.06659 (2017).

**DSOD**:

Shen, Zhiqiang, Zhuang Liu, Jianguo Li, Yu-Gang Jiang, Yurong Chen, and Xiangyang Xue. "Dsod: Learning deeply supervised object detectors from scratch." In The IEEE International Conference on Computer Vision (ICCV), vol. 3, no. 6, p. 7. 2017.

**RON**:

Kong, Tao, Fuchun Sun, Anbang Yao, Huaping Liu, Ming Lu, and Yurong Chen. "Ron: Reverse connection with objectness prior networks for object detection." In IEEE Conference on Computer Vision and Pattern Recognition, vol. 1, p. 2. 2017.

**RetinaNet**:

Lin, Tsung-Yi, Priya Goyal, Ross Girshick, Kaiming He, and Piotr Dollár. "Focal loss for dense object detection." arXiv preprint arXiv:1708.02002 (2017).

### Semantic Segmentation

**FCNs**:

Long, Jonathan, Evan Shelhamer, and Trevor Darrell. "Fully convolutional networks for semantic segmentation." In Proceedings of the IEEE conference on computer vision and pattern recognition, pp. 3431-3440. 2015.

**SegNet**:

Badrinarayanan, Vijay, Alex Kendall, and Roberto Cipolla. "Segnet: A deep convolutional encoder-decoder architecture for image segmentation." IEEE transactions on pattern analysis and machine intelligence 39, no. 12 (2017): 2481-2495.

**Dilated Convolutions**:

Yu, Fisher, and Vladlen Koltun. "Multi-scale context aggregation by dilated convolutions." In International Conference on Learning Representations, 2015.

**ParseNet**:

Liu, Wei, Andrew Rabinovich, and Alexander C. Berg. "Parsenet: Looking wider to see better." In CoRR. 2015.

**DeepLab**:

Liang-Chieh, Chen, George Papandreou, Iasonas Kokkinos, Kevin Murphy, and Alan Yuille. "Semantic image segmentation with deep convolutional nets and fully connected crfs." In International Conference on Learning Representations. 2015.

Chen, L. C., G. Papandreou, I. Kokkinos, K. Murphy, and A. L. Yuille. "DeepLab: Semantic Image Segmentation with Deep Convolutional Nets, Atrous Convolution, and Fully Connected CRFs." IEEE transactions on pattern analysis and machine intelligence (2017).

Chen, Liang-Chieh, George Papandreou, Florian Schroff, and Hartwig Adam. "Rethinking atrous convolution for semantic image segmentation." arXiv preprint arXiv:1706.05587 (2017).

Chen, Liang-Chieh, Yukun Zhu, George Papandreou, Florian Schroff, and Hartwig Adam. "Encoder-decoder with atrous separable convolution for semantic image segmentation." arXiv preprint arXiv:1802.02611 (2018).

**PSPNet**:

Zhao, Hengshuang, Jianping Shi, Xiaojuan Qi, Xiaogang Wang, and Jiaya Jia. "Pyramid scene parsing network." In IEEE Conf. on Computer Vision and Pattern Recognition (CVPR), pp. 2881-2890. 2017.

**ICNet**:

Zhao, Hengshuang, Xiaojuan Qi, Xiaoyong Shen, Jianping Shi, and Jiaya Jia. "Icnet for real-time semantic segmentation on high-resolution images." arXiv preprint arXiv:1704.08545 (2017).

**Global Convolutional Net**:

Peng, Chao, Xiangyu Zhang, Gang Yu, Guiming Luo, and Jian Sun. "Large Kernel Matters--Improve Semantic Segmentation by Global Convolutional Network." In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition, pp. 4353-4361. 2017.




