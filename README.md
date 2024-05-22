# Uncertainty in Self-supervised Depth Estimation Using Multi-scale Decoders

Mayank Mali

Written as the thesis document for 5th Year Masters in CS at CMU 2021-22.

## Abstract

Depth estimation is an image translation problem that predicts depth maps for a given camera image and has fostered research in various applications including self-driving vehicles. 
Self-supervised depth estimation methods are of particular interest since ground truth LIDAR depth is expensive to acquire and instead use view synthesis as weaker supervision. 
Generally, the produced depth maps to date are only point estimates of an underlying depth distribution due to randomness in model training, resulting in noisy depth estimates that 
can propagate errors and lead to inaccurate or fatal decisions in real-world applications. Recent interest has been sparked in reducing such noise by modeling the uncertainty of 
depth estimates. Empirical uncertainty strategies seek to predict uncertainty via statistical methods by treating independent models as black box predictors. Of particular interest 
are predictive strategies that seek to learn the inherent uncertainty of a depth model. For example, student-teacher frameworks train one network to learn the depth output 
distribution of another. Such methods are desirable due to the advantage of requiring fewer training and space resources compared to other empirical methods. In this work, we study 
self-supervised depth models with a U-Net architecture that outputs depths at multiple scales. In particular, we explore a novel predictive uncertainty model that only has access 
to these scales and the U-Net bottleneck feature. We evaluate and discuss the novel method alongside other uncertainty strategies on the KITTI dataset.
