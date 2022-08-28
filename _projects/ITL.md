---
layout: page
title:  Incremental Transfer Learning
description:  Incremental Learning Meets Transfer Learning, Application to Multi-site Prostate MRI Segmentation <br/><br/>
img: assets/img/ITL/visualization_res18.png
importance: 2
category: Research
---

**Keywords: Incremental Learning, Transfer Learning, Medical Image Segmentation**


**This paper has been accpted by [MICCAI-DECAF](https://decaf-workshop.github.io/decaf-2022/)**


Many medical datasets have recently been created for medical image segmentation tasks, and it is natural to question whether we can use them to sequentially train a single model that (1) performs better on all these datasets, and (2) generalizes well and transfers better to the unknown target site domain. Prior works have achieved this goal by jointly training one model on multi-site datasets, which achieve competitive performance on average but such methods rely on the assumption about the availability of all training data, thus limiting its effectiveness in practical deployment. In this paper, we propose a novel multi-site segmentation framework called **incremental-transfer learning (ITL)**, which learns a model from multi-site datasets in an end-to-end sequential fashion. Specifically, incremental refers to training sequentially constructed datasets, and transfer is achieved by leveraging useful information from the linear combination of embedding features on each dataset. In addition, we introduce our ITL framework, where we train the network including a site-agnostic encoder with pretrained weights and at most two segmentation decoder heads. We also design a novel site-level incremental loss in order to generalize well on the target domain. Second, we show for the first time that leveraging our ITL training scheme is able to alleviate challenging catastrophic forgetting problems in incremental learning. We conduct experiments using five challenging benchmark datasets to validate the effectiveness of our incremental-transfer learning approach. Our approach makes minimal assumptions on computation resources and domain-specific expertise, and hence constitutes a strong starting point in multi-site medical image segmentation.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ITL/model.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1: Overview of (a) our proposed Incremental Transfer Learning framework, and (b) the multi-site expert model. Note that in this study, we only use one multi-site expert model and one source decoder network, which will not introduce additional parameter.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ITL/visualization_res18.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 2: Visualization of segmentation results on five benchmarks using ResNet-18 as the encoder. Different site results are shown in different colors.
</div>


## Citation

{% raw %}
```bibtex
@article{you2022incremental,
  title={Incremental Learning Meets Transfer Learning: Application to Multi-site Prostate MRI Segmentation},
  author={You, Chenyu and Xiang, Jinlin and Su, Kun and Zhang, Xiaoran and Dong, Siyuan and Onofrey, John and Staib, Lawrence and Duncan, James S},
  journal={arXiv preprint arXiv:2206.01369},
  year={2022}
}
```
{% endraw %}



