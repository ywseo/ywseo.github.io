---
title: "A structureless approach for visual odometry"
collection: publications
permalink: /publication/2018-01-01-paper-title-number-3
excerpt: ''
date: 2018-04-01
venue: 'IV-18'
paperurl: 'https://ieeexplore.ieee.org/document/8500617'
---
A local, bundle-adjustment is an important procedure to improve the accuracy of a visual odometry solution.
However, it is computationally very expensive as it jointly
optimize all the poses of cameras and locations of map points.
To reduce the computational complexity of such a procedure
without much sacrificing the accuracy of a solution, the state-
of-the-art algorithms [1],[2],[3] were proposed to eliminate the
map point variables, using extra matrix operations, from their
linearized optimization solutions. Instead of eliminating the
map points, this paper proposes a novel way of addressing this
complexity issue – we represent a map point as a function
of two camera poses, and uses the triangulated location of
the map point when needed. Our method is more efficient
than a full-SLAM formulation in solving the visual odometry
problem in that 1) the complexity of our solution is lower
than those of the state-of-the-art methods, 2) no extra matrix
operations required to eliminate map points, 3) no need guesses
on map points’ initial locations. Experiemental results, through
simulated experiments and experiments with KITTI data,
demonstrated that our results are more accurate that those
of a full-SLAM approach with lower runtime complexities.

[Download paper here](https://ieeexplore.ieee.org/document/8500617)

Chih-Chung Chou, Chun-Kai Chang and **YoungWoo Seo**, A structureless approach for visual odometry, In <i>Proceedings of the IEEE Intelligent Vehicles Symposium</i> (IV-2018), pp. 1834-1841, 2018.
