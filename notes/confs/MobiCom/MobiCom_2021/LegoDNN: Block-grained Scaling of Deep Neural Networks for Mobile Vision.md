# Contributions ```C```:
Comprehensive evaluation on LegoDNN compared to existing methods using filter pruning, knowledge distillation or quantization.

---

**Quotes**

Fast generation of large scaling space via block re-training.

Fine-grained DNN scaling via block switching

---

# Takeaways

---

**Quotes**

Limitations of model-grained scaling. The key to achieve the full promise of accurate DNNs is to effectively scale their sizes in correspondence to the dynamics of available resource. Existing layer removing techniques [12, 31, 43, 44, 63] such as filter pruning require re-training of a model to mitigate its severe accuracy loss once its size is changed. However, these models only provide a coarse-grained differentiation of resources, often incurring large accuracy losses (Figure 1(a)) and leaving considerably propor- tions of resource unused (Figure 1(b)). 

Research question 3: how to optimally assemble descendant block on the fly?

LegoDNN measures the percentage of reduced latency compared to that of the original block.

Once any change of available resources is detected, the optimizer checks up all DNNs’ profiles of descendant blocks, and finds the optimal combination of these DNNs that maximizes the inference accuracy under the processing latency constraints.

A block’s processing latency is proportional to its block size, namely its number of parameters.

```Generic-categoryimagerecognition.```
```
VGG16, ResNet18
Cifar-10, ImageNet2012
```
```Real-time object detection and video analytic.```
```
YOLOv3
COCO2017
```

NestDNN improves this technique by judging a filter as important if its extracted feature maps can differentiate images of different classes [9].


---

**Miscellaneous**

Testbeds:

Smart phones (Huawei Mate20 X and Xiaomi 5S)

Embedded devices (Raspberry Pi 4B and Jetson TX2).

**Questions**

What is the specific definition of Sparsity?

What is Integer Linear Programming (ILP) problem?


