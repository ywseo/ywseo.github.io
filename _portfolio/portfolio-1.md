---
title: "Enabling Mobile Robots to Know Where They are at Any Given Time"
excerpt: "Tight coupling of vision-lidar measurements for effective odometry, visual odometry using pseudo map points, lateral localization for reliable, urban autonomous driving."
collection: portfolio
---

<img src="/images/tvlo-iv19.png"/>

**Tight coupling of vision-lidar measurements for effective odometry** This work is about a new way of fusing the visual and lidar measurements for effective odometry. When to combine visual measurements with lidar measurements, it is typical to assign the depth information from lidar measurements to seemingly corresponding, visual features or to utilize the results of visual odometry as the motion initial guess for lidar odometry. Instead, our method 1) builds two maps in different modalities: a lidar voxel map and a visual map with map-points and 2) use them together when to solve the odometry residuals. And the results of the odometry residual optimization are used to keep the lidar voxel map to be globally consistent with the operating environment. By using visual- lidar measurements in such a tightly-coupled way, our method estimates the odometry more accurately as incorporating more geometric constraints into the odometry residuals, and removes any chances of errors in assigning the depths of lidars to non- corresponding visual features. Experimental results show that our method outperforms the visual (i.e., the front-end of the ORB-SLAM2), and lidar odometry, and depth-enhanced visual odometry.
Read the following paper to learn more about this work:
* **YoungWoo Seo** and Chih-Chung Chou, [A tight coupling of vision-lidar measurements for effective odometry](https://ieeexplore.ieee.org/document/8814164), In *Proceedings of the 30th IEEE Intelligent Vehicles Symposium* (IV-2019), pp. 990-995, 2019.

------

<img src="/images/pseudo-map-points.png"/>

**Visual Odometry Using Pseudo Map Points** A local, bundle-adjustment is an important procedure to improve the accuracy of a visual odometry solution. However, it is computationally very expensive as it jointly optimize all the poses of cameras and locations of map points. To reduce the computational complexity of such a procedure without much sacrificing the accuracy of a solution, the state-of-the-art algorithms were proposed to eliminate the map point variables, using extra matrix operations, from their linearized optimization solutions. Instead of eliminating the map points, this paper proposes a novel way of addressing this complexity issue – we represent a map point as a function of two camera poses, and uses the triangulated location of the map point when needed. Our method is more efficient than a full-SLAM formulation in solving the visual odometry problem in that 1) the complexity of our solution is lower than those of the state-of-the-art methods, 2) no extra matrix operations required to eliminate map points, 3) no need guesses on map points’ initial locations. Experiemental results, through simulated experiments and experiments with KITTI data, demonstrated that our results are more accurate that those of a full-SLAM approach with lower runtime complexities.
Read the following paper to learn more about this work:
* Chih-Chung Chou, Chun-Kai Chang and **YoungWoo Seo**, [A structureless approach for visual odometry](https://ieeexplore.ieee.org/document/8500617), In *Proceedings of the 29th IEEE Intelligent Vehicles Symposium* (IV-2018), pp. 1834-1841, 2018.

------

<img src="/images/estimated-local-road-geometry.jpg"/>

**Lateral Localization for Reliable Urban Autonomous Driving** For safe urban driving, keeping a car within a road-lane boundary is a critical prerequisite. It requires human and robotic drivers to recognize the boundary of a road-lane and the vehicle's location with respect to the boundary of a road-lane that the vehicle happens to be driving on. To provide such a perception capability, we develop a new computer vision system that analyzes a stream of perspective images to produce information about a vehicle's location relative to the a road-lane's boundary, and information about the detecting of lane-crossing and lane-changing maneuvers. To assist the vehicle's lateral localization, our algorithm also estimates the host road-lane's geometry, including the number of road-lanes, their widths, and the index of the host road-lane. The local road geometry estimated by frame-by-frame may be inconsistent over frames, due to variations in the image features. To handle such inconsistent estimations, we implement an Unscented Kalman Filter (UKF) to smooth out, over time, the estimated road geometry. Tests on inter-city highway showed that our system provides stable and reliable performance in terms of computing lateral distances and detecting lane-crossing and lane-changing maneuvers. 
Read the following papers to learn more about this work:
* **Young-Woo Seo** and Myung Hwangbo, [A computer vision system for lateral localization](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.21576), *Journal of Field Robotics*, 32(7): 1004-1014, 2015.
* **Young-Woo Seo** and Raj Rajkumar, [Tracking and estimation of ego-vehicle's state for lateral localization](https://ieeexplore.ieee.org/document/6957859/), In *Proceedings of the 17th International IEEE Conference on Intelligent Transportation Systems* (ITSC-2014), pp. 1251-1257, Qingdao, China, Oct 8-11, 2014.
* **Young-Woo Seo** and Raj Rajkumar, [Use of a monocular camera to analyze a ground vehicle's lateral movements for reliable autonomous city driving](http://www.cs.cmu.edu/~youngwoo/doc/ppniv-13-ywseo.pdf), In *Proceedings of the 5th IEEE IROS Workshop on Planning, Perception and Navigation for Intelligent Vehicles* (PPNIV-2013), pp. 197-203, Nov 3-8, Tokyo, Japan, 2013.

<iframe width="560" height="315" src="https://www.youtube.com/embed/A09se5Z-s9A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
