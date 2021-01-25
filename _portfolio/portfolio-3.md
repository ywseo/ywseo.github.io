---
title: "Enabling Mobile Robots to Know What Objects Are Around"
excerpt: "Target-tracking for drone, moving object detection and tracking, generating instantaneous map around ground vehicles."
collection: portfolio
---

<img src="/images/en-kcf.png"/>

**Target-Tracking for Drone** Computer vision technologies are very attractive for practical applications running on embedded systems. For such applications, it is desirable for the deployed algorithms to run in high-speed and require no offline training. To develop a single-target tracking algorithm with these properties, we propose an ensemble of the kernelized correlation filters (KCF), we call it EnKCF. A committee of KCFs is specifically designed to address the variations in scale and translation of moving objects. To guarantee a high-speed run-time performance, we deploy each of KCFs in turn, instead of applying multiple KCFs altogether to each frame. To reduce any potential drifts between individual KCFs’ transition, we also developed a particle filter. Experimental results showed that the performance of ours is, on average, 70.10% for precision at 20 pixels, 53.00% for success rate for the OTB100 data, and 54.50% and 40.2% for the UAV123 data. Experimental results also demonstrated that our method is better than other high-speed trackers over 5% on precision on 20 pixels and 10-20% on AUC on average. Moreover, our implementation ran at 340 fps for the OTB100 and at 416 fps for the UAV123 dataset that is faster than DCF (292 fps) for the OTB100 and KCF (292 fps) for the UAV123. To increase flexibility of the proposed EnKCF running on various platforms, we also explored different levels of deep convolutional features. Read the following paper to learn more about this work: 
* Burak Uzkent and **YoungWoo Seo**, [EnKCF: Ensemble of kernelized correlation filter for high-speed object tracking](/files/enkcf.pdf), In *Proccedings of the IEEE Winter Conference on Applications of Computer Vision* (WACV-18), pp. 1133-1141, 2018.

------

<img src="/images/moving-object-detection-tracking.jpg"/>

**Moving Object Detection and Tracking** A self-driving car, to be deployed in real-world driving environments, must be capable of reliably detecting and effectively tracking of nearby moving objects. This paper presents our new, moving object detection and tracking system that extends and improves our earlier system used for the 2007 DARPA Urban Challenge. We revised our earlier motion and observation models for active sensors (i.e., radars and LIDARs) and introduced a vision sensor. In the new system, the vision module detects pedestrians, bicyclists, and vehicles to generate corresponding vision targets. Our system utilizes this visual recognition information to improve a tracking model selection, data association, and movement classification of our earlier system. Through the test using the data log of actual driving, we demonstrate the improvement and performance gain of our new tracking system. Read the following paper to learn more about this work:
* Hyunggi Cho, **Young-Woo Seo**, B.V.K. Vijaya Kumar, and Ragnunathan (Raj) Rajkumar, [A multi-sensor fusion system for moving object detection and tracking in urban driving environments](https://ieeexplore.ieee.org/document/6907100/), In *Proceedings of the IEEE International Conference on Robotics and Automation* (ICRA-14), pp. 1836-1843, 2014.

<iframe width="560" height="315" src="https://www.youtube.com/embed/XN4p6pqaDEU?ecver=1" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

------
 
<img src="/images/omni-view.jpg"/> 
 
 **Generating Instantaneous Map Around Ground Vehicles** To safely drive on urban streets, it is critical for self-driving cars to timely obtain the locations of other road occupants (e.g., cars, pedestrians, bicyclists, etc.). If such information is unreliably estimated, it would put a self-driving car in a great risk. To provide our self-driving car with such a capability, this work develops a perception algorithm that generates, by combining scan points from multiple, automotive grade LIDARs, temporally consistent and spatially seamless snapshots of neighboring (dynamic and static) objects. To do so, the proposed algorithm first represents a square region centered at the current location of ego-vehicle and then traces, for each of the LIDAR scans, a virtual ray between a LIDAR and the edge of reliable sensing range, to update cells on the ray. Through the tests with several urban streets driving data, the proposed algorithm showed promising results in terms of clearly identifying traversable regions in the drivable regions. Read the following paper to learn more about this work:
 * **Young-Woo Seo**, [Generating omni-directional view of neighboring objects for ensuring safe urban driving](https://www.ri.cmu.edu/publications/generating-omni-directional-view-of-neighboring-objects-for-ensuring-safe-urban-driving/), *Tech. Report CMU-RI-TR-14-11*, the Robotics Institute, Carnegie Mellon University, June, 2014.
 
 <iframe width="560" height="315" src="https://www.youtube.com/embed/ztK8lklLvLU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
