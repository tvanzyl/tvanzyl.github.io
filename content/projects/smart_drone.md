---
author: Terence L van Zyl
title: Mega Smart Savannahs
date: 2024-04-30
description: Mega Smart Savannahs
math: true
---

We recently joined forces with [Smart Savanahs](https://smartsavannahs.org/en/) to bring deep learning models into Sub-Saharan Africa.

<!--more-->

## Wildlife Tracking and Re-Identifcation With Drones

![Smart Savanahs](/images/Mega%20Smart%20Savannah.png)

### Purpose

> Identifying and tracking individuals in vast nature reserves is crucial for supporting wildlife biodiversity and welfare and addressing conflicts at the human-wildlife nexus, such as poaching. Drones with high-resolution cameras offer an efficient and scalable solution for providing observations of large, inaccessible and rugged terrain.
>
> Conservationists can deploy drones to capture detailed video footage, enabling targeted tracking and re-identification of specific individuals – animals, humans, or vehicles. Since individuals are often camouflaged, researchers can use advanced machine-learning models to detect specific wildlife species or even focus on identifying individual animals or humans based on unique markings or other characteristics. Machine learning can significantly aid in helping conservationists develop strategies to minimize human-wildlife conflict and directly support SDGs like Goal 15 (Life on Land). 

### How it works

> The drone (DJI Mavic Pro) captures a live video feed, which it transmits to the controller in real time. The controller sends the footage via an HDMI capture card (Magewell) to our Jetson Orin Nano. We have deployed an accelerated version of the [Mega Detector](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) model to the Jetson Orin Nano. We use [TensorRT](https://developer.nvidia.com/tensorrt) for the acceleration and [DeepStream](https://developer.nvidia.com/deepstream-sdk) for the object tracking pipeline. The live object detections are then streamed to a portal screen for real-time assisted wildlife identification and tracking.


### Use Cases

> **Targeted Tracking:** Drones can be used to follow specific herds or monitor the movement of individual animals of interest, providing valuable insights into their behavior, migration patterns, and potential threats.

> **Wildlife Re-identification:** The high-resolution imagery and ML analysis facilitate the reliable re-identification of individual animals, supporting conservation efforts, population monitoring, and anti-poaching measures.
 
> **Cost-Effective Monitoring:** Compared to ground-based surveys, drones offer a more cost-effective and time-efficient method for wildlife monitoring, especially over large or inaccessible areas.


