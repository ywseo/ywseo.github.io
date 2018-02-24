---
title: "Building lane-graphs for autonomous parking"
collection: publications
permalink: /publication/2010-10-01-paper-title-number-1
excerpt: ''
date: 2010-10-01
venue: 'IROS-10'
paperurl: 'http://ieeexplore.ieee.org/document/5650331/'
---
An autonomous robotic vehicle can drive through and park in a lot more reliably if it is guided by a parking lot map. This specialized map creates structure, including the centerlines of drivable regions and intersection locations in an often unstructured and unmarked environment and enables the vehicle to focus its attention on regions that require detailed analysis. Existing methods of building such maps require manu- ally driving vehicles for collecting sensor measurements. Instead of pursuing a labor-intensive approach, we analyze an aerial image of a parking lot to build a topological map. In particular, our algorithm produces a lane-graph of a parking lot's drivable regions by executing several image processing steps. First it estimates drivable regions by superimposing detection of a parking spots onto the parking lot boundary segmentation. Second, a distance transform is applied to drivable regions to reveal its skeleton. Lastly our algorithm searches the distance map to identify a set of the peak points and connects them to generate a lane-graph that concisely represents drivable regions. Experiments show promising results of real-world parking lot aerial-imagery analysis.

[Download paper here](http://ieeexplore.ieee.org/document/5650331/)

**Young-Woo Seo**, Chris Urmson, David Wettergreen, and Jin-Woo Lee, Building lane-graphs for autonomous parking, In <i>Proceedings of the IEEE International Conference on Intelligent Robots and Systems</i> (IROS-10), pp. 6052-6057, 2010. 