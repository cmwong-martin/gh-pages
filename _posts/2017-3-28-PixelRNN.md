---
title: Pixel RNN - predicts the pixels in an image
---

### Problem ###
To predict the pixels in an image. For example, if an image is occluded, PixelRNN will recover the occulded part within the image, as shown in the following:

![example image](/gh-pages/figure/PixelRNN/fig1.png){: .center-image }

### Proposed Method ###
Using two LSTMs for modeling two directions respectively: row and diagonal, as shown in the following:

![example image](/gh-pages/figure/PixelRNN/fig2.png){: .center-image }

### Advantages ###
1. model full dependencies between the collor channels.
2. model both spatially local and long-range correlations
3. produce sharp and coherent recovery

### Result ###

![example image](/gh-pages/figure/PixelRNN/fig3.png){: .center-image }

![example image](/gh-pages/figure/PixelRNN/fig4.png){: .center-image }

### Reference ###

1.  Oord, A. V. D., Kalchbrenner, N., & Kavukcuoglu, K. (2016). Pixel recurrent neural networks. arXiv preprint arXiv:1601.06759.
