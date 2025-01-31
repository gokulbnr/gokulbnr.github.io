---
title: "Enhancing Visual Place Recognition via Fast and Slow Adaptive Biasing in Event Cameras"
authors: Gokul B. Nair, Michael Milford, and Tobias Fischer
collection: publications
permalink: /publication/dvs-biasing-vpr
excerpt: 'This paper introduces feedback control algorithms that automatically tune the bias parameters through two interacting methods: 1) An immediate, on-the-fly fast adaptation of the refractory period, which sets the minimum interval between consecutive events, and 2) if the event rate exceeds the specified bounds even after changing the refractory period repeatedly, the controller adapts the pixel bandwidth and event thresholds, which stabilizes after a short period of noise events across all pixels (slow adaptation).'
date: 25-03-2024
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
paperurl: 'https://arxiv.org/pdf/2403.16425'
---

Event cameras are increasingly popular in robotics due to their beneficial features, such as low latency, energy efficiency, and high dynamic range. Nevertheless, their downstream task performance is greatly influenced by the optimization of bias parameters. These parameters, for instance, regulate the necessary change in light intensity to trigger an event, which in turn depends on factors such as the environment lighting and camera motion. This paper introduces feedback control algorithms that automatically tune the bias parameters through two interacting methods: 1) An immediate, on-the-fly fast adaptation of the refractory period, which sets the minimum interval between consecutive events, and 2) if the event rate exceeds the specified bounds even after changing the refractory period repeatedly, the controller adapts the pixel bandwidth and event thresholds, which stabilizes after a short period of noise events across all pixels (slow adaptation). Our evaluation focuses on the visual place recognition task, where incoming query images are compared to a given reference database. We conducted comprehensive evaluations of our algorithms' adaptive feedback control in real-time. To do so, we collected the QCR-Fast-and-Slow dataset that contains DAVIS346 event camera streams from 366 repeated traversals of a Scout Mini robot navigating through a 100 meter long indoor lab setting (totaling over 35km distance traveled) in varying brightness conditions with ground truth location information. Our proposed feedback controllers result in superior performance when compared to the standard bias settings and prior feedback control methods. Our findings also detail the impact of bias adjustments on task performance and feature ablation studies on the fast and slow adaptation mechanisms.

[![Read on Paper](https://img.shields.io/badge/Read%20the%20Paper-Download-blue?style=for-the-badge&logo=arxiv)](https://arxiv.org/pdf/2403.16425)
[![DOI](https://img.shields.io/badge/Read%20the%20Paper-IEEE%20Xplore-blue?style=for-the-badge&logo=openaccess)](https://ieeexplore.ieee.org/document/10802384)
<!-- [![Watch the Video](https://img.shields.io/badge/Watch%20the%20Video-Play-red?style=for-the-badge&logo=youtube)](https://www.youtube.com/watch?v=8D9gtHqteEQ) -->
[![Dataset](https://img.shields.io/badge/Dataset-Available-green?style=for-the-badge&logo=databricks)](https://huggingface.co/datasets/gokulbnr/QCR-Fast-Slow-Event-Dataset)
[![Code](https://img.shields.io/badge/Code-Available-blue?style=for-the-badge&logo=github)](https://github.com/gokulbnr/fast-slow-biased-event-vpr/tree/main)

<iframe width="560" height="315" src="https://www.youtube.com/embed/8D9gtHqteEQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


```bibtex
@inproceedings{nair2024enhancing,
  title={Enhancing Visual Place Recognition via Fast and Slow Adaptive Biasing in Event Cameras},
  author={Nair, Gokul B and Milford, Michael and Fischer, Tobias},
  booktitle={Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  year={2024}
}
```
