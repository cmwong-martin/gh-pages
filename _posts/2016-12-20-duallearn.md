---
title: Dual Learning Mechanism - train your translation model without any human labelling
---

### Problem ###
It is very expensive to manually **label tens of millions of bilingual sentence pairs** for training your machine-translation model.


### Proposed Method ###
Consider the following two figures,

  1. A model $$M1$$ translates English sentence to target French sentence.
  ![example image](/gh-pages/figure/dual_learning/fromEToF.png){: .center-image }
  2. Another model $$M2$$ translates French sentence to target English sentence. ![example image](/gh-pages/figure/dual_learning/fromFToE.png){: .center-image }

The learning of the proposed method [1] is shown in the following steps, and given an English sentence $$x$$,

1. the model $$M1$$ translates $$x$$ to French sentence $$y$$.
2. immediately, the model $$M2$$ translates $$y$$ to $$x'$$.
3. at last, the model $$M1$$ will check whether $$x'$$ equals to $$x$$.

A reinforcement learning (i.e. policy gradient) is employed to train both $$M1$$ and $$M2$$ simultaneously.

### Advantages ###
The learning of the model is based on **unlabel bilingual sentence pairs** which can be obtained massively.

### Disadvantages ###
It is expected that using reinforcement learning for the proposed method is time-comsunimg.

### Result ###

![example image](/gh-pages/figure/dual_learning/re1.png){: .center-image}

![example image](/gh-pages/figure/dual_learning/re2.png){: .center-image}

![example image](/gh-pages/figure/dual_learning/re3.png){: .center-image}


### Reference ###

1.  Yingce Xia, Di He, Tao Qin, Liwei Wang, Nenghai Yu, Tie-Yan Liu, and Wei-Ying Ma, Dual
learning for machine translation, CoRR abs/1611.00179 (2016).
