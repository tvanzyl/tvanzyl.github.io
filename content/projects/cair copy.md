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

> Traditional methods of tracking and identifying wildlife, especially over large areas, are costly and labor-intensive. Drones equipped with high-resolution cameras offer a more efficient and scalable solution for targeted tracking and re-identification of specific species.
> 
> Drones can be deployed to capture detailed aerial imagery of specific areas of interest. Since individual animals can be relatively small compared to the overall landscape, advanced machine learning (ML) algorithms are used to analyze these images. These algorithms can be trained to detect specific wildlife species, such as elephants, rhinos, or giraffes, with a focus on individual identification based on unique markings or other characteristics. While ML might not perfectly identify every animal, it can assist in pinpointing individuals for further tracking and re-identification across different sightings.

### How it works

> The drone (DJI Mavic Pro) captures a live video feed, which it transmits to the controller in real time. The controller sends the footage via an HDMI capture card (Magewell) to our Jetson Orin Nano. We have deployed an accelerated version of the [Mega Detector](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) model to the Jetson Orin Nano. We use [TensorRT](https://developer.nvidia.com/tensorrt) for the acceleration and [DeepStream](https://developer.nvidia.com/deepstream-sdk) for the object tracking pipeline. The live object detections are then streamed to a portal screen for real-time assisted wildlife identification and tracking.


### Use Cases

> **Targeted Tracking:** Drones can be used to follow specific herds or monitor the movement of individual animals of interest, providing valuable insights into their behavior, migration patterns, and potential threats.

> **Wildlife Re-identification:** The high-resolution imagery and ML analysis facilitate the reliable re-identification of individual animals, supporting conservation efforts, population monitoring, and anti-poaching measures.
 
> **Cost-Effective Monitoring:** Compared to ground-based surveys, drones offer a more cost-effective and time-efficient method for wildlife monitoring, especially over large or inaccessible areas.


