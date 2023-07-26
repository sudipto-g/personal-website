---
title: "Multi-Object Tracker"
date: 2019-05-12T12:14:34+06:00
image: "images/portfolio/item-1.png"
client: "John Doe"
project_url : "https://https://github.com/sudipto-g/TrackEA"
categories: ["development"]
description: "A Multi-Object Tracker through different frames of reference"
draft: false
---

#### Project Requirements

Most object tracking systems consider the video as “motion picture” or, a set of images projected one after the other, at a very high frame rate.  
Consequently, the Object Tracking modules available in most Open Source libraries, eg: OpenCV work in the following way (at a meta level):  
In the video stream, the first frame is captured  
A Region of Interest (RoI) selection is made based on the initial frame  
The region selected in the previous step is tracked through the next frames  
Thus, these methods of tracking objects work fine, so long as the object remains within the frame.  
As soon as the objects move out of the frame, no longer is the tracking valid.  
Further, in some adaptive trackers, once the objects move out of frame, they may not be recognised even if they reappear in future frames, as adaptive trackers keep updating their state based on the current ground truth data i.e. current video frame.  

Thus, this makes vanilla Object Tracking highly unsuitable for tracking objects that need to be continuously monitored. For eg: Traffic Data.  

Thus, to address the above issues, a very simple strategy was adopted.  


#### Project Details

An re-initialisation policy was used, everytime a certain number of objects move out of the frame.  
For instance, in Traffic Survelliance systems, the initial frame is captured and cars/vehicles in the initial frame are detected using the YOLOv3 detector. This corresponds to the ROI selection step.  
Next, the detected objects are tracked through the remaining frames and as soon as a “fixed number” of vehicles (this “fixed number” can be set by the user) move out of the frame, the tracking is re-initialised.  
That is, the object detector is run again to select the current ROI and thus, all the problems of a vanilla Object Tracker, spoken of in the Project Requirements section is addressed.  
