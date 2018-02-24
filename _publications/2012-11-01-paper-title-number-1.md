---
title: "Exploiting publicly available cartographic resources for aerial image analysis"
collection: publications
permalink: /publication/2012-11-01-paper-title-number-1
excerpt: ''
date: 2012-11-01
venue: 'GIS-12'
paperurl: 'https://dl.acm.org/citation.cfm?doid=2424321.2424336'
---
Cartographic databases can be kept up to date through aerial image analysis. Such analysis is optimized when one knows what parts of an aerial image are roads and when one knows locations of complex road structures, such as overpasses and intersections. This paper proposes self-supervised computer vision algorithms that analyze a publicly available cartographic resource (i.e., screenshots of road vectors) to, without human intervention, identify road image-regions and detects overpasses. 
Our algorithm segments a given input image into two parts: road- and non-road image regions. It does so not by learning a global appearance model of roads from hand-labeled data, but rather by approximating a locally consistent model of the roads' appearance from self-obtained data. In particular, the learned local model is used to execute a binary classification. We then apply an MRF to smooth potentially inconsistent binary classification outputs. 
To detect overpasses, our method scrutinizes screenshots of road vector images to approximate the geometry of the underlying road vector and use the estimated geometry to localize overpasses. 
Our methods, based on experiments using inter-city highway ortho-images, show promising results. Segmentation results showed on average over 90% recall; overpass detection results showed 94% accuracy.

[Download paper here](https://dl.acm.org/citation.cfm?doid=2424321.2424336)

**Young-Woo Seo**, Chris Urmson and David Wettergreen, Exploiting publicly available cartographic resources for aerial image analysis, In <i>Proceedings of the ACM SIG SPATIAL International Conference on Advances in Geographic Information System</i> (GIS-12), pp. 109-118, 2012. 