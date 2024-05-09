# Operation Pixel Merge
You assume the role of Fleet Admiral Reinhard von Lohengramm, leading the Galactic Empire’s forces in a crucial war. You have recently received a transmission from one of your captains, most likely containing some very important information regarding the ongoing war but alas it seems to be split into a hundred different images!

Create a script using OpenCV and Pillow, utilizing some clever image recognition and manipulation techniques to stitch together these fragmented parts to reveal the secret message!

## Overview
The assets folder in this repository has a bunch of images, each of dimensions 512x512 pixels. Each one is composed of a white background with a **singular** coloured dot on it. The images are named with a number indicating their order in the sequence. 

There are also few images which are completely white, the importance of these will be discussed further down.

## Instructions
* Sort the images by the number specified in the filename
* Use OpenCV to detect the dot on each image and record its coordinates as well as its colour
* Use Pillow to draw a line between the dot on one image and the dot on the succeeding image
    * The colour of the line should be governed by the colour of the starting dot
* The pure white images represent a line break. I.e. you should not draw to it from a previous image

## Resources
* [OpenCV](https://docs.opencv.org/4.x/)
* [Pillow](https://pillow.readthedocs.io/en/stable/reference/ImageDraw.html)
