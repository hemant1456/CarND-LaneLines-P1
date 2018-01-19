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

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

I followed the approach mentioned in the tutorial videos, I did parameter tuning using experimentation and intution.

for extrapolation i separated my x,y values based on two factors-
1) slope 2) x value should be less than middle of maximum x value
Then i got y values for those x after fitting a line on x,y and drew lines on image


### 2. Identify potential shortcomings with your current pipeline


It will not work on circular paths


### 3. Suggest possible improvements to your pipeline

Use neural network for automatic feature detection of road so that it works on circular paths also.
