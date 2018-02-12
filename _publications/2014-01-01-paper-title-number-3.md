---
title: "Utilizing instantaneous driving direction for enhancing lane-marking detection"
collection: publications
permalink: /publication/2014-01-01-paper-title-number-3
excerpt: ''
date: 2014-05-01
venue: 'IV-14'
paperurl: 'http://ieeexplore.ieee.org/document/6856467/'
---
Our earlier lane-marking detection method identified lane-markings appearing on an input image based on the intensity contrast between lane-markings pixels and their neighboring pixels. This detection results in outputs with nearly-zero false negatives, but with many false positives. To filter out these false positives in a principled way, we utilize the driving direction of a roadway. We do this because longitudinal lane-markings delineate the driving direction of a road and the orientations of any true, longitudinal lane-markings appearing on input images should be aligned with this direction. To approximate the driving direction of a road, we detect the vanishing point on a horizon line and draw a line to link the image coordinates of the detected vanishing point to those of the center of the image bottom. We then filter out any lane-marking blobs if their orientations are not aligned with that of the approximated driving direction. Through testing with streets and inter-city highway images, the proposed method demonstrates its effectiveness.

[Download paper here](http://ieeexplore.ieee.org/document/6856467/)

Young-Woo Seo and Ragnunathan (Raj) Rajkumar, Utilizing instantaneous driving direction for enhancing lane-marking detection, In <i>Proceedings of the IEEE Intelligent Vehicles Symposium</i> (IV-14), pp. 170-175, 2014. 