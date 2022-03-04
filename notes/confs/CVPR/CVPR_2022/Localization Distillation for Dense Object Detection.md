# Contributions ```C```:
The authors propose and investigate using localization distillation to teach a student network, which shows that knowledge distillation is more important than semantic knowdedge (soft class labels) when distilling object detectors.

# Takeaways
It can be better to use {t, b, l, r} instead of {x, y, w, h} to regress bounding boxes, as the physical meaning of the former {t, b, l, r} is consistent, each of which is border of a bounding box.

# Questions
Not sure how dense is the soft-bounding box for KL.

# Miscellaneous
It would be great to test how small/lightweight the network can be.

