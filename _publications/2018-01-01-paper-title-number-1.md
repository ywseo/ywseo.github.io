---
title: "EnKCF: Ensemble of kernelized correlation filter for high-speed object tracking"
collection: publications
permalink: /publication/2018-01-01-paper-title-number-1
excerpt: ''
date: 2018-03-01
venue: 'WACV-18'
paperurl: 'https://ieeexplore.ieee.org/document/8354233/'
---
Computer vision technologies are very attractive for practical applications running on embedded systems. For such an application, it is desirable for the deployed algorithms to run in high-speed and require no offline training. To develop a single-target tracking algorithm with these properties, we propose an ensemble of the kernelized correlation filters (KCF), we call it EnKCF. A committee of KCFs is specifically designed to address the variations in scale and translation of moving objects. To guarantee a high-speed run-time performance, we deploy each of KCFs in turn, instead of applying multiple KCFs to each frame. To reduce any potential drifts between individual KCFs’ transition, we developed a particle filter. Experimental results showed that the performance of ours is, on average, 70.10% for precision at 20 pixels, 53.00% for success rate for the OTB100 data, and 54.50% and 40.2% for the UAV123 data. Experimental results showed that our method is better than other high-speed trackers over 5% on precision on 20 pixels and 10-20% on AUC on average. Moreover, our implementation ran at 340 fps for the OTB100 and at 416 fps for the UAV123 dataset that is faster than DCF (292 fps) for the OTB100 and KCF (292 fps) for the UAV123. To increase flexibility of the proposed EnKCF running on various platforms, we also explored different levels of deep convolutional features.

[Download paper here](https://ieeexplore.ieee.org/document/8354233/)

Burak Uzkent and **YoungWoo Seo**, EnKCF: Ensemble of kernelized correlation filter for high-speed object tracking, In <i>Proccedings of the IEEE Winter Conference on Applications of Computer Vision</i> (WACV-18), pp. 1133-1141, 2018.
