---
title: "Detection and Tracking of Stop-Lines"
collection: work
permalink: /work/2014-10-01-work-title-number-7
excerpt: ''
date: 2014-10-01
venue: ''
paperurl: ''
---
To be successfully deployed in real world driving environments, self-driving cars should be capable of complying with the traffic rules, i.e., understanding rules in place and executing its driving maneuvers as dictated. For example, an autonomous vehicle should be able to recognize stop-lines and stop at the detected stop-line. Such a capability is a crucial one that self-driving cars must acquire, to drive along with manually-driven cars. To develop such a perception capability, this work aims at developing a computer vision algorithm that detects, through an analysis of the detected lane-markings' geometric layout, stop-lines and tracks, using an unscented Kalman filter, the detected stop-line over time. To detect lateral and longitudinal lane-markings, our method applies a spatial filter emphasizing the intensity contrast between lane-marking pixels and their neighboring pixels. We then examine the detected lane-markings to identify perpendicular, geometry layouts between longitudinal and lateral lane-markings for stop-line detection. To provide reliable stop-line recognition, we developed an unscented Kalman filter to track the detected stop-line over frames. Through the testings with real-world, busy urban street videos, our method demonstrated promising results, in terms of the accuracy of the initial detection accuracy and the reliability of the tracking.
