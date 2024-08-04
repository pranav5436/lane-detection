# Lane Detection and Car Tracking Project

This project is focused on lane detection and car tracking using OpenCV and Python. The program reads a video file, processes each frame to detect lanes, and overlays the detected lanes on the original frames. The processed video is then saved as an output video file.

## Requirements

- Python 3.x
- OpenCV
- NumPy

## Installation

1. Install Python 3.x from [python.org](https://www.python.org/).
2. Install the required libraries using pip:

```bash
pip install opencv-python numpy


Usage
Clone the repository or download the source code.
Update the video_path and output_path variables in the script to point to your input video file and desired output location.
Run the script:

python lane_detection.py



Code Explanation
Import Libraries: Import the necessary libraries - OpenCV for computer vision tasks and NumPy for array operations.

Define Functions:

region_of_interest(img, vertices): Masks the region of interest in the image.
draw_the_lines(img, lines): Draws lines on the image based on the detected lines from the Hough transform.
Main Script:

Set the video_path and output_path.
Capture the video from the specified path using cv2.VideoCapture.
Define the codec and create a VideoWriter object to save the output video.
Process each frame:
Convert the frame to grayscale.
Apply Canny edge detection.
Mask the region of interest.
Detect lines using the Hough transform.
Draw the detected lines on the original frame.
Display the resulting frame.
Save the processed frame to the output video.
Release the video capture and writer objects and close all OpenCV windows.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Author
This project was created by Pranav Shukla.

© Pranav Shukla
