# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describing my pipeline.

My pipeline consisted of 6 steps. 

First, I converted the images to grayscale. 
Second, I applied a GaussianBlur.
Third, I applied the Canny transform.
Fourth, I applied an image mask to keeps the region of the image defined by the polygon formed from `vertices`.
Fifth, I applied Hough Line Transform to detect lines in an image.
Sixth, I applied LinearRegression to approximation lines.  
Then I drew lines on image.

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be inaccurate detecting of the marking line you near area. 


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to make better approximation of the marking line.

