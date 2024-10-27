# [CVPR 2023] Zero-Shot Object Counting


 
<!---
<div style="display: flex;">
  <img src="./figures/ZSC.gif" alt="Second Image" style="width: 60%;"> 
</div>
-->

Counting without human annotated exemplars.

## Overview
This repository contains the implementation of the paper [**Zero-Shot Object Counting**](https://arxiv.org/abs/2303.02001). 
We propose zero-shot object counting (ZSC), a new setting where only the class name is available during test time. Such a counting system does not require human annotators in the loop and can operate automatically. Starting from a class name, we propose a method that can accurately identify the optimal patches which can then be used as counting exemplars. We first construct a class prototype to select the patches that are likely to contain the objects of interest and then we train a model to quantitatively measure how suitable an arbitrary patch is as a counting exemplar. By applying this model to all the candidate patches, we can select the most suitable patches as exemplars for counting.

 <img src="./figures/pipeline.png" alt="Pipeline" style="width: 70%;">

## Links:
Please follow this link to download: "regressor_model/regressor.pth", box_rpn_all.npy, and box_rpn_sel_all.npy:

https://drive.google.com/drive/folders/1FjkaK2EzcOdiH_N9WkGnh5c3G9xj9PmE?usp=drive_link

## Bib
Please cite our CVPR 2022 paper:
```
@InProceedings{Xu_2023_CVPR,
    author    = {Xu, Jingyi and Le, Hieu and Nguyen, Vu and Ranjan, Viresh and Samaras, Dimitris},
    title     = {Zero-Shot Object Counting},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2023},
    pages     = {15548-15557}
}
```

## Acknowledgment
This repo heavily based on [BMNet]([https://link-url-here.org](https://github.com/flyinglynx/Bilinear-Matching-Network)https://github.com/flyinglynx/Bilinear-Matching-Network). Thanks for the great work.
