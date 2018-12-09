---
title: "Enabling Self-Driving Cars to Know Where They Can and Cannot Drive"
excerpt: "Tracking of traversable region boundary, lanemarking detection, vanishing point tracking for road geometry understanding, analyzing ortho-images to generate lane-level maps."
collection: portfolio
---

<img src="/images/boundary-detection.jpg"/>

**Tracking Traversable Region Bounary** This work presents a new method of detecting
and tracking the boundaries of drivable regions in road without
road-markings. As unmarked roads connect residential places
to public roads, a capability of autonomously driving on such
roadways is important to truly realize self-driving cars in daily
driving scenarios. To detect the left and right boundaries of
drivable regions, our method samples the image region at the
front of ego-vehicle and uses the appearance information of that
region to identify the boundary of the drivable region from in-
put images. Due to variation in the image acquisition condition,
the image features necessary for boundary detection may not
be present. When this happens, a boundary detection algorithm
working frame-by-frame basis would fail to successfully detect
the boundaries. To effectively handle these cases, our method
tracks, using a Bayes filter, the detected boundaries over frames.
Experiments using real-world videos show promising results. Read the following paper to learn more about this work:
* **Young-Woo Seo** and Raj Rajkumar, [Detection and tracking of boundary of unmarked roads](https://ieeexplore.ieee.org/document/6916256/?arnumber=6916256), In *Proceedings of the 17th International Conference on Information Fusion* (Fusion-2014), Salamanca, Spain, 2014.

<br>

<img src="/images/instantaneous-driving-direction.png"/> 

**Lanemarking Detection** In advanced driver assistance systems and self-driving cars, many computer vision applications rely on knowing the location of the vanishing point on a horizon. The horizontal vanishing point's location provides important information about driving environments, such as the instantaneous driving direction of roadway, sampling regions of the drivable regions' image features, and the search direction of moving objects. To detect the vanishing point, many existing methods work frame-by-frame. Their outputs may look optimal in that frame. Over a series of frames, however, the detected locations are inconsistent, yielding unreliable information about roadway structure. This work studys a novel algorithm that, using lines, detects vanishing points in urban scenes and, using Extended Kalman Filter (EKF), tracks them over frames to smooth out the trajectory of the horizontal vanishing point. The study demonstrates both the practicality of the detection method and the effectiveness of our tracking method, through experiments carried out using thousands of urban scene images. Read the following papers to learn more about this work:
* **Young-Woo Seo** and Raj Rajkumar, [Detection and tracking of the vanishing point on a horizon for automotive applications](http://www.cs.cmu.edu/~youngwoo/doc/ppniv-14-ywseo.pdf), In *Proceedings of the 6th IEEE IROS Workshop on Planning, Perception and Navigation for Intelligent Vehicles* (PPNIV-2014), Chicago, Sep 14-18, 2014.
* **Young-Woo Seo** and Raj Rajkumar, [Utilizing instantaneous driving direction for enhancing lane-marking detection](https://ieeexplore.ieee.org/document/6856467/), In *Proceedings of the 25th IEEE Intelligent Vehicles Symposium* (IV-2014), pp. 170-175, Dearborn, MI, 2014.
 
<br> 

<img src="/images/uc-starting-chute.png"/>

**Analyzing Ortho-Images to Generate Lane-Level Maps** Maps are important for both human and robot navigation. Given a route, driving assistance systems consult maps to guide human drivers to their destinations. Similarly, topological maps of a road network provide a robotic vehicle with information about where it can drive and what driving behaviors it should use. By providing the necessary information about the driving environment, maps simplify both manual and autonomous driving. The majority of existing cartographic databases are built, using manual surveys and operator interactions, to primarily assist human navigation. Hence, the resolution of existing maps is insufficient for use in robotics applications. Also, the coverage of these maps fails to extend to places where robotics applications require detailed geometric information. To augment the resolution and coverage of existing maps, this work investigates computer vision algorithms to automatically build lane-level detailed maps of highways and parking lots by analyzing publicly available cartographic resources such as orthoimagery. Read the following papers to learn more about this work:
* **Young-Woo Seo**, David Wettergreen, and Chris Urmson, [Exploiting publicly available cartographic resources for aerial image analysis](https://dl.acm.org/citation.cfm?doid=2424321.2424336), In *Proceedings of the ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems* (GIS-2012), pp. 109-118, Redondo Beach, CA, 2012.
* **Young-Woo Seo**, David Wettergreen, and Chris Urmson, [Ortho-image analysis for producing lane-level highway maps](https://dl.acm.org/citation.cfm?doid=2424321.2424401), In *Proceedings of the ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems* (GIS-2012), pp. 506-509, Redondo Beach, CA, 2012. 
* **Young-Woo Seo**, Chris Urmson, David Wettergreen, and Jin-Woo Lee, [Building lane-graphs for autonomous parking](https://ieeexplore.ieee.org/document/5650331/), In *Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems* (IROS-2010), pp. 6052-6057, Taipei, Taiwan, 2010.
* **Young-Woo Seo**, Chris Urmson, David Wettergreen, and Rahul Sukthankar, [Adapting to intra-class variations using incremental retraining with exploratory sampling](https://www.ri.cmu.edu/publications/adapting-to-intra-class-variations-using-incremental-retraining-with-exploratory-sampling/), *Tech Report CMU-RI-TR-10-36*, Oct, 2010.
* **Young-Woo Seo**, Chris Urmson, David Wettergreen, and Jin-Woo Lee, [Augmenting cartographic resources for autonomous driving](https://dl.acm.org/citation.cfm?doid=1653771.1653777), In *Proceedings of the ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems* (GIS-2009), pp. 13-22, Seattle, WA, November, 2009.
* **Young-Woo Seo** and Chris Urmson, [Utilizing prior information to enhance self-supervised aerial image analysis for extracting parking lot structures](https://ieeexplore.ieee.org/document/5354405/), In *Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems* (IROS-2009), pp. 339-344, St. Louis, MO, October, 2009. 
* **Young-Woo Seo**, Nathan Ratliff, and Chris Urmson, [Self-supervised aerial image analysis for extracting parking lot structure](http://ijcai.org/Proceedings/09/Papers/305.pdf), In *Proceedings of the Twenty-First International Joint Conference on Artificial Intelligence* (IJCAI-2009), pp. 1837-1842, Pasadena, CA, July, 2009.
 
