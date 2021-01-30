# Contributions ```C```:
A generic top-down approach for human pose tracking and Re-ID, i.e., it first detect human and then perform human pose estimation. Siamese Graph Convolution Network is used for human pose keypoints  matching and Re-ID.

For Re-ID problem, use keypoints for matching because for online matching a visual classifier is expensive.
Spatial and pose consistency are used for identity association.

# Limitations ```L```:
Only one previous frame is used for Re-ID. For long temporal dependency it requires other techniques such as LSTM, RNN to extract temporal features in longer history.
