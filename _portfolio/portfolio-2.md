---
title: "Understanding Computational Workload of Self-Driving Car"
excerpt: "Analysis of CPU utilization <br/>[](images/software-architecture.jpg)"
collection: portfolio
---

#### Understanding Computational Workload of Self-Driving Car

To enable a vehicle to drive autonomously, a computing unit of a self-driving car must be capable of running many software tasks (e.g., motion-planning, moving object detection, etc.) in parallel. As those tasks are computationally intensive and the capacity of a computing unit is not unbounded, it is important to efficiently utilize such limited computational resources. To this end, this study aims at developing a method that predicts the CPU usage patterns of software tasks running on a self-driving car. To ensure safety of such dynamic systems, the worst-case-based CPU utilization analysis has been used; however, the nature of dynamically changing driving contexts requires more flexible approach for an efficient computing resource management. To better understand the dynamic CPU usage patterns, this study presents an effort of designing a feature vector to represent the information of driving environments and of predicting, using regression methods, the selected tasks' CPU usage patterns given specific driving contexts. Experiments with real-world vehicle data show a promising result and validate the usefulness of the proposed methods.</br></br>
Read the following papers to learn more about this work:
* Young-Woo Seo, Junsung Kim, and Raj Rajkumar, [Predicting dynamic computational workload of a self-driving car](https://ieeexplore.ieee.org/document/6974391/), In *Proceedings of the IEEE International Conference on Systems, Man, and Cybernetics* (SMC-2014), pp. 3030-3035, San Diego, CA, Oct 5-8, 2014.
* Junsung Kim, Young-Woo Seo, Hyoseung Kim, and Raj Rajkumar, [Can cyber-physical systems to be predictable? inferring cyber-workloads from physical attributes](https://ieeexplore.ieee.org/document/6843732/), In *Proceedings of the ACM/IEEE International Conference on Cyber-Physical Systems* (ICCPS-2014), 2014. 
