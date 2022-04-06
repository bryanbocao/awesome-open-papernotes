# Takeaways

---

**Quotes**

A detection model may only involve a few classes, with which much less knowledge can be distilled from inter-class similarity of teacher’s softened outputs

Detectors care more about local regions that overlap with ground truth objects while classification models pay more attention to global context. So directly doing full feature imitation would unavoidably introduces large amount of noise from uncared areas, especially for object detection where background instances are overwhelming and diverse.

Recall in knowledge distillation, relative probabilities on different classes indeed tell a lot about how the teacher model tends to generalize.

For practical speedups, weight pruning needs support of sparse computations and quantization relies on low-bit operations.

This method utilizes inter-location discrepancy of teacher’s feature response on near object anchor locations for distilling the knowledge in cumber- some detection models. Our Intuition is that the discrep- ancy of feature response on the near object anchor locations reveals important information of how large detector tends to generalize, with which learned knowledge can be distilled.

We add the adaptation layer for two reasons: 1) The student feature’s channel number may not be compatible with teacher model. The added layer can align the former to the later for calculating distance metric. 2) We find even when student and teacher have compatible features, forcing student to approximate teacher feature directly leads to minor gains compared to the adapted counterpart.

Shufflenet [39] which gives excellent classification performance with limited flops and parameters. However, the Shufflenet architecture itself is dedicated for image classification. We find directly adapting it to detection produces terrible result. This is because each point on the top feature map has an equivalent stride of 32, leading to very coarse alignment of anchor boxes on the input images. Moving to lower output layer with smaller stride also performs not well as features are less powerful therein.

Object detection requires higher resolution feature to make downstream feature decoder (the detector heads) work well.

Grouped detection of near objects is a common error case for the raw student model.

---

**Questions**

In Section 4.1, the authors say "detection heads use full convolution", what does "full convolution" specifically mean?
