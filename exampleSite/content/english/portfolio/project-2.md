---
title: "Facial Keypoints Detector"
date: 2019-05-12T12:14:34+06:00
image: "images/portfolio/item-3.png"
project_url : "https://github.com/sudipto-g/Facial_Keypts_Detector"
categories: ["ml", "development"]
description: "This is meta description."
draft: false
---

#### Introduction

An attempt at building a Facial Key Points Detector.  
Facial keypoints include points around the eyes, nose, and mouth on a face and can used for facial tracking, facial pose recognition, facial filters, and emotion recognition.  

#### The Pipeline

Given a picture, faces in it are detected using a [Haar-Cascade.](https://towardsdatascience.com/face-detection-with-haar-cascade-727f68dafd08)  
Next, on each of the localised faces, some cropping, standardisation, normalisation and resizing techniques are applied before presenting it to the facial key point recogniser.  
The keyoint recogniser runs a CNN to warp the image and maps it to 68 key points.  

#### A Demo

The input image:  

![Input Image](https://sudipto-g.github.io/Facial_Keypts_Detector/Figure_1.png)


The detected faces (Haar Casacde detects some aberrant faces) Detected Faces:  

![Detected Faces](https://sudipto-g.github.io/Facial_Keypts_Detector/Figure_3.png)


And then, finally, the detected keypoints of my own face:  

![Detected Keypoints](https://sudipto-g.github.io/Facial_Keypts_Detector/Figure_2.png)

Thus, this is an example of my Facial Keypoint Detector being applied to my own image :p
