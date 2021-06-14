# OpenCV-Counter

A simple application using OpenCV to detect the amount of people going in certain directions off of a cam feed.

## Required libraries

* NumPy
* OpenCV
* dlib
* imutils
* SciPy

# How it works

There are two "phases" to the program: detecting, and tracking

The system works upon the principle of *skipped frames:* For every predefined number of frames that have passed, the frame after will be the more computationally expensive frame

## Detecting

Detecting uses OpenCV along with elements from pyimagesearch (custom module) in order to have a computationally expensive tracker that is accurate to 97 percent

## Tracking

Tracking is the less computationally espensive element, this uses Euclidean models in order to determine the distance between two or more objects and calculate the next frame to which they will move- the majority of the algorithm uses this as it is less expensive
