---
title: Structural RNN - Modeling Spatio-Temporal Graphs
---

### Problem ###
Recurrent Neural network works well in time or sequence modeling, but spatial modeling. Structural RNN takes account into both spatial and temporal information of the data.  



### Proposed Method ###
Each timestep to RNN is represented by a graph of different objects as shown in the following. Each objects will represent a node in RNN.

![example image](/gh-pages/figure/structureRNN/fig2.png){: .center-image }

![example image](/gh-pages/figure/structureRNN/fig1.png){: .center-image }

### Advantages ###
1. model spatial and temporal relationship

### Disadvantages ###
1. heavy annotation of the data may require

### Result ###

![example image](/gh-pages/figure/PixelRNN/fig3.png){: .center-image }

![example image](/gh-pages/figure/PixelRNN/fig4.png){: .center-image }

### Reference ###

1.  Jain, A., Zamir, A. R., Savarese, S., & Saxena, A. (2016). Structural-RNN: Deep learning on spatio-temporal graphs. In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (pp. 5308-5317).
