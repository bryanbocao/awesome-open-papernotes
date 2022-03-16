# Contributions ```C```:
A method to train a compressed student model from a large general (or essemble of) (a) teacher model(s) by KL divergence on sotf-targets and temperature to control to what extend distillation pays attention to negative logits.

# Takeaways

---

**Quotes**

If the cumbersome model generalizes well because, for example, it is the average of a large ensemble of different models, a small model trained to generalize in the same way will typically do much better on test data than a small model that is trained in the normal way on the same training set as was used to train the ensemble.


For tasks like MNIST in which the cumbersome model almost always produces the correct answer with very high confidence, much of the information about the learned function resides in the ratios of very small probabilities in the soft targets.

At lower temperatures, distillation pays much less attention to matching logits that are much more negative than the average. On the other hand, the very negative logits may convey useful information about the knowledge acquired by the cumbersome model. Which of these effects dominates is an empirical question. We show that when the distilled model is much too small to capture all of the knowledege in the cumbersome model, intermedi- ate temperatures work best which strongly suggests that ignoring the large negative logits can be helpful.

Our distillation approach is able to extract more useful information from the training set than simply using the hard labels to train a single model. More than 80% of the improvement in frame classification accuracy achieved by using an ensemble of 10 models is trans- ferred to the distilled model.

---

