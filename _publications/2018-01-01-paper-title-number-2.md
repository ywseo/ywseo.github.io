---
title: "A two-stage sampling for robust feature matching"
collection: publications
permalink: /publication/2018-01-01-paper-title-number-2
excerpt: ''
date: 2018-01-01
venue: 'JFR'
paperurl: 'http://onlinelibrary.wiley.com/doi/10.1002/rob.21778/abstract'
---
For any visual feature based SLAM solutions, to estimate the relative camera motion between two images, it is necessary to find “correct” correspondence between features extracted from those images. Given a set of feature correspondents, one can use a n-point algorithm with robust estimation method, to produce the best estimate to the relative camera pose. The accuracy of a motion estimate is heavily dependent upon the accuracy of the feature correspondence. Such a dependency is even more significant when features are extracted from the images of the scenes with drastic changes in viewpoints and illuminations, and presence of occlusions. To make a feature matching robust to
such challenging scenes, we propose a new feature matching method that incrementally chooses a five pairs of matched features for a full DoF camera motion estimation. In particular, at the first stage, we use our 2-point algorithm to estimate a camera motion, and at the second stage, use this estimated motion to choose three more matched features. In addition, we use, instead of the epipolar constraint, a planar constraint for more accurate outlier rejection. With this set of five matching features, we estimate a full DoF (Degree of Freedom) camera motion with scale ambiguity. Through the experiments with three, real-world datasets, our method demonstrates its effectiveness and robustness by successfully matching features 1) from the images of a night market where presenceof frequent occlusions and varying illuminations, 2) from the images of a night market taken by a handheld camera and by the Google street view, and 3) from the images of a same location taken daytime and nighttime.

[Download paper here](http://onlinelibrary.wiley.com/doi/10.1002/rob.21778/abstract)

Chih-Chung Chou, **YoungWoo Seo**, and Chieh-Chih Wang, A two-stage sampling for robust feature matching, <i>Journal of Field Robotics</i>, 35(5): 779-801, 2018.
