#**Advanced Lane Finding** 

---
##**Build a Advanced Lane Finding Project**

### the approach taken for this project

1,calibrate function is using all of the chess images to collect more data for calibrating, that using the computer vision technical to find the straight line

2,undistort function is changing the image to a plane using the result of the calibrating process

3,colorGradient function is finding the different pixels by control the sensitivity of the algorithm, that can find the line of lane

4,perspectiveTransformWarper function is changing the image from any sight to the eagle's sight 

5,findLine function is using the window searching method to find the line of lane on the road,and the cover a different color on the lane

6,radius_curv function is calculating the radius of the lane

7,process_image function is the pipline of image handling

### discussion 

when the pipeline to fail, the smooth detection process can be used for check the lane.

because the lane always has same width usually, if there is some situations that the width of lane is change too large, so it must be some thing error.

after the error occurs, the edge of lane can be averaged by the line we found before.

the important parameter and image can be saved every times when handle the image, and also can save many frame of the video.

so at that time, we can use the parameter and image saved before to handle the exception situations