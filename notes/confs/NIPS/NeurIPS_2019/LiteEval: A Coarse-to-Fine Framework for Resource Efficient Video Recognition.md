# Takeaways

---

**Quotes**

###### Motivation
In addition to network design, the computational cost of CNNs is directly affected by input resolution—74% of computation can be saved (measured by floating point operations) when evaluating a ResNet-101 model on images with half of the original resolution, while still offering reasonable accuracy.

###### Intuition
Intuitively, during inference, lightweight modules are run by default to recognize easy samples (e.g., images with canonical views) with coarse scale inputs and high-precision components will be activated to further obtain finer details to recognize hard samples.

The most expensive operation in the framework is to compute CNN features from video frames, while LSTMs are much more computationally efficient—only 0.06% of GFLOPs needed to extract features with a
ResNet-101 model


---

**TODO**

Check GumbelMax trick.
v1.3 split
