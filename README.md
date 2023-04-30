### Road Lane Line Detection using Computer Vision  

#### Overview  
When we drive, we use our eyes to decide where to go. The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle. Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm. <br>

To detect lane lines we will be using Python and OpenCV. OpenCV means "Open-Source Computer Vision", which is a package that has many useful tools for analyzing images.  <br>
  
The tools we have are color selection, region of interest selection, grayscaling, Gaussian smoothing, Canny Edge Detection and Hough Tranform line detection. We will build a pipeline to detect the line segments in images, then average/extrapolate them and draw them onto the images for display. Once we do this successfully for images, we will apply this to video.  

#### Our strategy to solve this:
1. Detect lane lines manually using numpy & matplotlib <br>
   i. Color selection (select lane colors - white and yellow) <br>
   ii. Region masking (select region of interest where the lane lines appear) <br>
2. Detect road lane lines using OpenCV  <br>
   i. Gray scale <br>
   ii. Gaussian Smoothing <br>
   iii. Canny Edge Detection <br>
   iv. Region Masking <br>
   v. Hough Transform <br>
3. Apply on different test images
4. Apply on Singapore road lane
5. Apply on Video
6. Apply on Singapore road lane video