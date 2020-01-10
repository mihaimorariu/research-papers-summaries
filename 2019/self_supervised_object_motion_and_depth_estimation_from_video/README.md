# Self-supervised Object Motion and Depth Estimation from Video

- Self-supervised learning framework
- Estimate individual object motion and monocular depth from video
- Previous approaches use dense 2D optical flow, or 3D scene flow to model the motion, meaning a pixel-wise flow map is predicted
  - Predict a 6-DoF rota-translation for the motion of individual object
  - The number of values to be estimated is significantly reduced from a pixel-wise prediction to 6 scalars per instance
- Solve the scale ambiguity in the view-synthsis based framework, using the pre-computed absolute camera ego-motion and the left-right photometric
loss
- The system estimates the combined transformation, encapsulatig both the camera ego-motion and the object motion
- The system system predicts absolute object motion which can be used to transform the object in 3D space directly

