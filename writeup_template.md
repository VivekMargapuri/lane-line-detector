# **Finding Lane Lines on the Road** 


**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report



---

### Reflection

Being new to pyhton, it was initially hard to code down and modify the draw_lines function. To fully understand what needs to be done to create an ideal pipeline, I slowly tuned and played with each of the functions on each of the image.

### 1.My Pipeline.

My pipeline consisted of 5 steps. 
First, I blacked out all the pixels except for yellow and white pixels.
Second step is to convert the image into grayscale.
Third step is to smoothen the grayscale image by gaussian_blur().
Fourth step is to apply canny edge detection.
Fifth step is to mark or create the region of interest.
Sixth step is to detect the hough lines.
Seventh step is to draw lines. I modified the draw_lines() function such that, the lines are filtered by slope into right lane or left lane segments. Then I used linear regression on these segments to create the line's equation. 

### 2. Shortcomings

The pipeline that I've created produces jumpy lines. Additionally, it may fail during low light conditions when the lines are not clearly visible.

### 3. Improvements
I aim to improve the smoothness of the lines. Probably, this has something to do with my draw_lines function. The regression model needs to be improved to make it work better for the curves lane lines.


