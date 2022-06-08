# Contributions ```C```:
---

**Quotes**

A high-resolution object detection framework. The key techniques in Remix are **adaptive partitioning** that generates partition plans to maximize the accuracy within a latency
budget through **non-uniform partitioning**; and **selective execution** that deals with short-term content dynamics and runs a partition plan efficiently.

---

# Takeaways

---

**Quotes**

17 object detection NNs based on five typical backbones: EfficientDet [69, 70], RetinaNet [37, 48], Faster-RCNN [64], YOLO [63], and SSD-MobileNet [53, 66].

###### Experimental Setup
PANDA: 555 images and 15 video sequences. Considering common camera and edge compute capability, we resize images and videos from the original resolution of 26,753×15,052 into 3,840×2,160 (4K).
Train/Test ratio: 80/20.

###### Observations
(1) Down-sampling inputs reduces the latency but has a low accuracy.

(2) Up-scaling networks increases the accuracy but has a high Latency.
- The accuracy of NNs varies among objects of different sizes. Overall, NNs obtain higher detection accuracy as object size increases.

(3) More importantly, marginal accuracy gain from different neural networks varies significantly across object sizes.

###### Opportunities and Challenges
Existing methods lack of spatial distribution of objects selection of diverse NNs.
Intuitively, for large objects in sparse scenes, a small and cheap NN should be used to reduce the latency, while for small objects in crowded scenes, a large and
expensive NN is desired to ensure high accuracy. -> contrary to my intuition.

Existing uniform partitioning treats every pixel equally by spending the same amount of computing power on each pixel.

However, when down sampled to 320×320, the input size of SSD-MobileNet, nearly half of the objects are smaller than 2.8 2 pixels, which is way too small to be detected by existing neural networks.

Leverage the previous detection results as the feedback to dynamically determine which blocks can be skipped in the current frame (§3.2.1).

---

**TODO**
Check e Soft-NMS, attenuation.
Understand 1) one-stage detectors: YOLOX [11], FCOS [48], DETR [65], Scaled-YOLOv4 [51], EfficientDet [45]. 2) two-stage detectors: VFNet [59], CenterNet2 [62]. 3) anchor-based detectors.
