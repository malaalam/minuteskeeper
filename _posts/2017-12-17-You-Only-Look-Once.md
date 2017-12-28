---
layout: post
title: You Only Look Once
categories: deepLearning
tags: YOLO, CNN
comments: true
---

<p><figure><a href="https://www.youtube.com/watch?v=VOC3huqHrss"><img src="/images/2017-12-17/YOLO.JPG" alt=""/></a><figcaption>
   [You Only Look Once (YOLO): Unified, Real-Time Detection]</figcaption></figure></p>

Recently, I came across this explosive video in which YOLO is applied for detecting multiple objects in a chase sequence in *Skyfall*. I was instantly taken up with the algorithm, became keen to figure out how it is implemented and to test it on my collection of photos and videos.

As one of its founders *Joseph Redmon* explains [here](https://www.youtube.com/watch?v=NM6lrxy0bxs), YOLO provides a dramatic increase in speed for a slight reduction in accuracy on the test-set. According to him, the YOLO algorithm processes images every **22 milliseconds** - during which period a vehicle being driven at 60 miles per hour can cruise 2 feet in distance. The next fastest option is the *Faster R-CNN* technique, which takes 140 milliseconds to process an image, so YOLO is around seven times faster for a comparable level of accuracy. (It makes me wonder, what is a good number of frames per second above which the human eye perceives a sequence of discrete images as a continuous video!)

YOLO is based on the *Sliding Window* principle. In the basal form of the Sliding Window, the image in question is looked at through a smaller window, probabilities for detecting any objects within that window are evaluated, and then the window is shifted by a bit along the image and the process is repeated. This process is effective but slow since the convolution network is run for each position of the sliding window. Fortunately much of the information obtained from each individual position of the window is repetitive. YOLO makes use of this to run the convolution network only once, which in turn gives its name!



