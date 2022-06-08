# Takeaways

---

**Quotes**

Tinier-YOLO is designed by introducing the **fire module** of SqueezeNet into Tiny-YOLO-V3 at first in order to reduce the model size. And then the number of fire models and their positions in the network architecture have been studied. The connectivity method between fire modules in Tinier-YOLO is realized by using **dense connections** of DenseNet. The **dense connections** in Tinier-YOLO helped to improve the detection accuracy and real-time performance. By incorporating the ```passthrough layer``` in Tinier-YOLO, the detection accuracy has been further improved by merging feature maps from the front layers to get fine-grained features.

The fire module of SqueezeNet uses the ```bottleneck layer``` network to compress the model and the network module is widened without losing detection accuracy heavily.

The SqueezeNet [31] proposed by UC Berkeley and Stanford researchers introduced **fire module**. The idea of fire module was similar to the series of Inception. It utilized **1\*1 convolutional layer** to compress the dimension of feature maps with the purposed to reduce parameters.

YOLO performed worse in location and detecting objects of small size. SSD discretized the output space of bounding boxes into a set of default boxes over different aspect ratios and scales per feature map location.

---
