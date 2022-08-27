---
layout: page
title: Balanced Incremental Approach for Meta Learning
description: Balanced Incremental Approach for Meta Learning
img: assets/img/MAML/Overview.png
importance: 3
category: Research
---

We present a novel Balanced Incremental Model Agnostic Meta Learning system
([BI-MAML](https://arxiv.org/pdf/2006.07412.pdf)) for learning multiple tasks. Our method implements a meta-update
rule to incrementally adapt its model to new tasks without forgetting old tasks.
Such a capability is not possible in current state-of-the-art MAML approaches.
These methods effectively adapt to new tasks, however, suffer from ’catastrophic
forgetting’ phenomena, in which new tasks that are streamed into the model degrade
the performance of the model on previously learned tasks. Our system performs
the meta-updates with only a few-shots and can successfully accomplish them.
Our key idea for achieving this is the design of balanced learning strategy for
the baseline model. The strategy sets the baseline model to perform equally well
on various tasks and incorporates time efficiency. The balanced learning strategy
enables BI-MAML to both outperform other state-of-the-art models in terms of
classification accuracy for existing tasks and also accomplish efficient adaption to
similar new tasks with less required shots. We evaluate BI-MAML by conducting
comparisons on two common benchmark datasets with multiple number of image
classification tasks. BI-MAML performance demonstrates advantages in both
accuracy and efficiency. [More about our paper](https://www.youtube.com/watch?v=4qlb-iG5SFo).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MAML/Baseline.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1. Baseline
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MAML/FineTuning.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 2. FineTuning
</div>

{% raw %}
```bibtex
@article{zheng2020bi,
  title={Bi-maml: Balanced incremental approach for meta learning},
  author={Zheng, Yang and Xiang, Jinlin and Su, Kun and Shlizerman, Eli},
  journal={arXiv preprint arXiv:2006.07412},
  year={2020},
  arxiv={2006.07412},
}


```
{% endraw %}
