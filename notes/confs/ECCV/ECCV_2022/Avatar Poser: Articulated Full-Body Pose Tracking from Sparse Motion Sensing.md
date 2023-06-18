# Contributions ```C```:
---
First learning-based approach to using only the head and hands in the upper bodies.

**Limitations of Prior Works**

Add additional sensors at the pelvis or lower body. Assume the knowledge of the pelvis pose.
For learning-based methods especially Transformer-based ones, they do that in offline setting where the motion information in the complete time domain is available.

**Key Notes from Related Work**

CoolMoves: First to use only the headset and hand-held controllers to estimate full-body poses. KNN-based on specific motion activities, thus unclear to scale to
larger datasets.

LoBSTr: GRU-based.

VAE-based.

METRO: First Transformer-based model.

PoseFormer & ST-Transformer: capture both body joint correlations and temporal dependencies.

MHFormer: spatial-temporal representations.
