# An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale

Link: https://arxiv.org/pdf/2010.11929v1.pdf
Publising Date: Oct 22, 2020
Read Date: Jun 2, 2021
Score /5: ⭐️⭐️⭐️⭐️
Status: First Read Through
Type: Academic Journal

> Paper Abstract: While the Transformer architecture has become the de-facto standard for natural language processing tasks, its applications to computer vision remain limited. In vision, attention is either applied in conjunction with convolutional networks, or used to replace certain components of convolutional networks while keeping their overall structure in place. We show that this reliance on CNNs is not necessary and a pure transformer applied directly to sequences of image patches can perform very well on image classification tasks. When pre-trained on large amounts of data and transferred to multiple mid-sized or small image recognition benchmarks (ImageNet, CIFAR-100, VTAB, etc.), Vision Transformer (ViT) attains excellent results compared to state-of-the-art convolutional networks while requiring substantially fewer computational resources to train.

- Key points:
    - Pure Transformer Architecture apply to Image Classification problem
    - Interpret an image as a sequence of patches and process it by a standard
    Transformer encoder as used in NLP
    - No application for other tasks of Computer Vision, such as detection and segmentation
    - Achieve SOTA with fewer computational costs
    - Larger model performs worst than smaller model on small datasets. On large datasets, the situation is inverted
    - Hybrid solution, with input as feature map from ResNet, but the improvement over pure Transformer is somehow subtle
    - Still, a large gap occurs between self-supervised learning and large-scale supervised pre-training
- Dataset:
    - CIFAR10/100
    - ImageNet
    - JFT