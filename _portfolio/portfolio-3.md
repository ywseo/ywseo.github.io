---
title: "Enabling Mobile Robots to Know What Objects Are Around"
excerpt: "target-tracking for drone, moving object detection and tracking, lanemarking detection, vanishing point tracking for road geometry understanding, generating instantaneous map around ground vehicles."
collection: portfolio
---

<img src="/images/en-kcf.png"/>

Computer vision technologies are very attractive for practical applications running on embedded systems. For such an application, it is desirable for the deployed algorithms to run in high-speed and require no offline training. To develop a single-target tracking algorithm with these properties, we propose an ensemble of the kernelized correlation filters (KCF), we call it EnKCF. A committee of KCFs is specifically designed to address the variations in scale and translation of moving objects. To guarantee a high-speed run-time performance, we deploy each of KCFs in turn, instead of applying multiple KCFs to each frame. To reduce any potential drifts between individual KCFs’ transition, we developed a particle filter. Experimental results showed that the performance of ours is, on average, 70.10% for precision at 20 pixels, 53.00% for success rate for the OTB100 data, and 54.50% and 40.2% for the UAV123 data. Experimental results showed that our method is better than other high-speed trackers over 5% on precision on 20 pixels and 10-20% on AUC on average. Moreover, our implementation ran at 340 fps for the OTB100 and at 416 fps for the UAV123 dataset that is faster than DCF (292 fps) for the OTB100 and KCF (292 fps) for the UAV123. To increase flexibility of the proposed EnKCF running on various platforms, we also explored different levels of deep convolutional features. Read the following paper to learn more about this work: 
* Burak Uzkent and **YoungWoo Seo**, [EnKCF: Ensemble of kernelized correlation filter for high-speed object tracking](https://arxiv.org/pdf/1801.06729.pdf), In *Proccedings of the IEEE Winter Conference on Applications of Computer Vision* (WACV-18), pp. 1133-1141, 2018.

<img src="/images/moving-object-detection-tracking.jpg"/>

A self-driving car, to be deployed in real-world driving environments, must be capable of reliably detecting and effectively tracking of nearby moving objects. This paper presents our new, moving object detection and tracking system that extends and improves our earlier system used for the 2007 DARPA Urban Challenge. We revised our earlier motion and observation models for active sensors (i.e., radars and LIDARs) and introduced a vision sensor. In the new system, the vision module detects pedestrians, bicyclists, and vehicles to generate corresponding vision targets. Our system utilizes this visual recognition information to improve a tracking model selection, data association, and movement classification of our earlier system. Through the test using the data log of actual driving, we demonstrate the improvement and performance gain of our new tracking system. Read the following paper to learn more about this work:
* Hyunggi Cho, **Young-Woo Seo**, B.V.K. Vijaya Kumar, and Ragnunathan (Raj) Rajkumar, [A multi-sensor fusion system for moving object detection and tracking in urban driving environments](https://ieeexplore.ieee.org/document/6907100/), In *Proceedings of the IEEE International Conference on Robotics and Automation* (ICRA-14), pp. 1836-1843, 2014.

<img src="/images/instantaneous-driving-direction.png"/> 

In advanced driver assistance systems and self-driving cars, many computer vision applications rely on knowing the location of the vanishing point on a horizon. The horizontal vanishing point's location provides important information about driving environments, such as the instantaneous driving direction of roadway, sampling regions of the drivable regions' image features, and the search direction of moving objects. To detect the vanishing point, many existing methods work frame-by-frame. Their outputs may look optimal in that frame. Over a series of frames, however, the detected locations are inconsistent, yielding unreliable information about roadway structure. This work studys a novel algorithm that, using lines, detects vanishing points in urban scenes and, using Extended Kalman Filter (EKF), tracks them over frames to smooth out the trajectory of the horizontal vanishing point. The study demonstrates both the practicality of the detection method and the effectiveness of our tracking method, through experiments carried out using thousands of urban scene images. Read the following papers to learn more about this work:
* **Young-Woo Seo** and Raj Rajkumar, [Utilizing instantaneous driving direction for enhancing lane-marking detection](https://ieeexplore.ieee.org/document/6856467/), In *Proceedings of the 25th IEEE Intelligent Vehicles Symposium* (IV-2014), pp. 170-175, Dearborn, MI, 2014.
* **Young-Woo Seo** and Raj Rajkumar, [Detection and tracking of the vanishing point on a horizon for automotive applications](http://www.cs.cmu.edu/~youngwoo/doc/ppniv-14-ywseo.pdf), In *Proceedings of the 6th IEEE IROS Workshop on Planning, Perception and Navigation for Intelligent Vehicles* (PPNIV-2014), Chicago, Sep 14-18, 2014.
* **Young-Woo Seo** and Raj Rajkumar, [Use of a monocular camera to analyze a ground vehicle's lateral movements for reliable autonomous city driving](http://www.cs.cmu.edu/~youngwoo/doc/ppniv-13-ywseo.pdf), In *Proceedings of the 5th IEEE IROS Workshop on Planning, Perception and Navigation for Intelligent Vehicles* (PPNIV-2013), pp. 197-203, Nov 3-8, Tokyo, Japan, 2013.
 
<img src="/images/omni-view.jpg"/> 
 
 To safely drive on urban streets, it is critical for self-driving cars to timely obtain the locations of other road occupants (e.g., cars, pedestrians, bicyclists, etc.). If such information is unreliably estimated, it would put a self-driving car in a great risk. To provide our self-driving car with such a capability, this work develops a perception algorithm that generates, by combining scan points from multiple, automotive grade LIDARs, temporally consistent and spatially seamless snapshots of neighboring (dynamic and static) objects. To do so, the proposed algorithm first represents a square region centered at the current location of ego-vehicle and then traces, for each of the LIDAR scans, a virtual ray between a LIDAR and the edge of reliable sensing range, to update cells on the ray. Through the tests with several urban streets driving data, the proposed algorithm showed promising results in terms of clearly identifying traversable regions in the drivable regions. Read the following paper to learn more about this work:
 * **Young-Woo Seo**, [Generating omni-directional view of neighboring objects for ensuring safe urban driving](https://www.ri.cmu.edu/publications/generating-omni-directional-view-of-neighboring-objects-for-ensuring-safe-urban-driving/), *Tech. Report CMU-RI-TR-14-11*, the Robotics Institute, Carnegie Mellon University, June, 2014.
 * **Young-Woo Seo** and Chris Urmson, [A perception mechanism for supporting autonomous intersection handling in urban driving](https://ieeexplore.ieee.org/document/4651162/), In *Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems* (IROS-2008), pp. 1830-1835, Nice, France, September, 2008.