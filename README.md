# Billards Assistant System Based on LabVIEW

## 1. Introduction

**Topics:** _Hough Circle Detection_, _Edge Detection_, _Algorithm Design_

**Skills:** _OpenCV_, _C++_, _LabVIEW_

This is the course project for `Virtual Experimental System Based on LabVIEW` and my final score for the course is **96/100**.

This is a teamwork and my teammates are _Weishu Chen_ and _Han Huang_.

My contributions in the project are:

- To find out the feasible algorithms for ball detection. To achieve this, I use the color `histogram` to find out the background color first, then I `binarize` the image, rendering the background black and the rest part white. As a matter of fact, `OpenCV` offers the function `HoughCircle` which is adequate for our task of detecting the balls on the binarized images;

- To design the algorithms for stick detection and table edge detection. I have tried the `Sobel operator`, the `Canny edge detector`, the `LSD algorithm` and the `EDLine algorithm` and none of them is practically competent for our tasks. So I designed my own algorithms that can produce favorable outcome;

- To design the algorithm to calculate the path of the balls;

- To build the "prototype". I tested my ideas and algorithms in `C++` first, and then my teammates transplant the code to the `LabVIEW` platform.

## 2. Demo

Here is the workflow of our project:

- Generate a binarized image. Use `HoughCircle` to detect balls:

![](/Asset/fig1.png)

- Estimate the range of the table:

![](/Asset/fig3.png)

- Estimate the location of the stick:

![](/Asset/fig4.png)

- Draw ball path:

![](/Asset/fig5.png)
