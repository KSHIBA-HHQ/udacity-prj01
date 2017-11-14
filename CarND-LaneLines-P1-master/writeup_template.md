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

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]

>> My pipeline consisted of 7 steps.
>> 1st.  converted the images to grayscale, 
>> 2nd.  Processed images with Gaussian filter
>> 3rd.  Processed images with Cany filter
>> 4th.  Processed images with Hough-P 
>> 5th.  Make continuous-lines from intermittent-lines
>> 5th.  Select the closest line in the left area
>> 6th.  Select the closest line in the right area
>> 7th.  Masking both-lines


### 2. Identify potential shortcomings with your current pipeline

>> Delete invalid part from intermittent-lines

One potential shortcoming would be what would happen when ... 

>>  When multiple intermittent lines appear simultaneously, the correct line is lost
    (Hough-P's shortcoming )


Another shortcoming could be ...

>>  Mask-area shifts at slopes and corners


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

>>  Improvement of my 5th step and 6th step

Another potential improvement could be to ...

>>  Correct using vehicle travel information
