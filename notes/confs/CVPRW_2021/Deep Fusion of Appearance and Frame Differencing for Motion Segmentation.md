# Contributions ```C```:
The authors propose to use a frame-differencing approach to do motion segmentation.

# Takeaways
## Comparison
Frame-differencing is more computationally efficient than 3D convolutional neural networks and has a better capability of capturing small objects due to smoothing or regularization.

# Questions
Inputs of the networks are the entire image, if we are only interested in RoI of moving objects, can we reduce the network size by only feeding RoI of moving objects?
Hasn't investigated the problem from an efficiency perspective. 

# Miscellaneous
[ResNet50 keras](https://keras.io/api/applications/) size: 98MB, 58.2 Time (ms) per inference step (CPU).
