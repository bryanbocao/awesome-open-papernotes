# Contributions ```C```:
First to up-scale Vision Transformers to larger size and reach new start-of-the-art results.

# Takeaways

---

**Quotes**

(1) Scaling up compute, model and data together improves representation quality.

(2) Representation quality can be bottlenecked by model size. Small models are not able to benefit from either the largest dataset, or compute resources.

(3) Large models benefit from additional data, even beyong 1B images. When increasing the dataset size, we observe a performance boost with big models, 
but not small ones. For small models, however, such at Ti/6 or B/32, increasing the dataset size does not help.

Relationship between compute and performance follows a power-law (E=aC<sup>b</sup>), resulting in a straight line on the log-log plot. If we extrapolate
from our observations, an infinite capacity model will obtain a non-zero error. This effect has also been observed for generative models [14].

Storing momentum in half-precision (bfloat16 type) does not affect training dynamics and has no effect on the outcome.

Larger models are much more sample efficient and are great few-shot learners.

---

# Limitations ```L```:
Not sure if these observations can generalize beyong the family of ViT models as mentioned by the authors.

# Questions
What does "saturate" mean specifically?
