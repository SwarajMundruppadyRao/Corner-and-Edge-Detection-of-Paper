# Corner-and-Edge-Detection-of-Paper

# Description
 To find the 4 corners of the paper using Edge Detection, Hough Transform and Corner Detection. This project was carried out as a part of Project 2 of ENPM673 course.

# Dependencies 

1. cv2
2. matplotlib
3. math


# Installing Dependencies

   ```bash
   sudo apt update
   sudo apt install python3-opencv python3-matplotlib
   ```

# Pipeline 

1. Read the video and extract individual frames using OpenCV.
2. Skip blurry frames (use Variance of the Laplacian and decide a suitable threshold)
3. Segment out the unwanted background area
4. Detect edges pixels in each frame using Canny Edge Detector
5. Use the detected edge pixels to extract straight lines in each frame using Hough Transform
6. Filter out “short” lines and only keep a few dominant lines.
7. Compute the intersections of the Hough Lines – these are the putative corners of the paper.
8. Verify the existence of those corners with Harris corner detector.
9. Filter out remaining extraneous corners that are not the 4 corners of the paper.
10. Generate the output video in which you have to overlay the 4 blue boundary lines and 4 red corners of the paper in each frame (excluding the blurry frames)


#Video

https://github.com/user-attachments/assets/f68e628c-0abe-4e1f-aa86-7e95fdcc11da


