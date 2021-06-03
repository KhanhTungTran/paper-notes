# Oscar: Object-Semantics Aligned Pre-training for Vision-Language Tasks

Author: Xiujun Li et al.
Github: https://github.com/microsoft/Oscar
Link: https://arxiv.org/pdf/2004.06165.pdf
Publising Date: Jul 26, 2020
Read Date: Jun 3, 2021
Score /5: ⭐️⭐️⭐️⭐️
Status: First Read Through
Type: Academic Journal

> Paper Abstract: Large-scale pre-training methods of learning cross-modal representations on image-text pairs are becoming popular for vision-language tasks. While existing methods simply concatenate image region features and text features as input to the model to be pre-trained and use self-attention to learn image-text semantic alignments in a brute force manner, in this paper, we propose a new learning method Oscar, which uses object tags detected in images as anchor points to significantly ease the learning of alignments. Our method is motivated by the observation that the salient objects in an image can be accurately detected, and are often mentioned in the paired text. We pre-train an Oscar model on the public corpus of 6.5 million text-image pairs, and fine-tune it on downstream tasks, creating new state-of the-arts on six well-established vision-language understanding and generation tasks.

- Key points:
    - Multi-modal and Generic model
    - Transformer Architecture apply to a wide-range of vision-language (V+L) tasks
    - Pre-train (VLP) then fine-tuning on task-specific data to achieve SOTA results of the tasks. The goal of pre-training is to learn cross-modal representations of image-text pairs in a self-supervised manner
    - Define the training samples as triples, each consisting of a word sequence, a set of object tags, and a set of image region features
    - Uses object tags as anchor points to align the image and language modalities in a shared semantic space
    - 2 type of tasks:
        - Understanding: VQA, GQA, NLVR2, Image-Text Retrieval, Text-Image Retrieval
        - Generation: Image Captioning, Novel Object Captioning
- Dataset:
    - COCO
    - MS COCO
    - Open Images
    - Many more for 7 different tasks