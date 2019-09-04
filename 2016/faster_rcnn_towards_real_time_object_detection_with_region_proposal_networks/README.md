# Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks

- _Region Proposal Network (RPN)_ for generating proposals
    - Predicts object bounds and objectness scores at each position
        - Anchors for addressing different scales and aspect ratios
    - Trained end-to-end to generate high-quality region proposals, which are used by Fast R-CNN for detection
- RPN and Fast R-CNN share convolutional features (one network)

![Network architecture](images/architecture.jpg "Network architecture")
