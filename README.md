Project Overview
This project contains code that automatically replaces billboards in video content with a new advertisement image. Using computer vision techniques, the program identifies the billboard area in each frame of the video and replaces it with a specified ad image, ensuring the replacement looks smooth and natural.

Directory Structure
The dataset for this project is organized into three folders:

train/ - Contains training video frames or datasets used to train object detection models.
test/ - Contains test videos for validating the trained model.
valid/ - Contains validation data to assess model performance before testing.
ad_image/ - Contains the advertisement image used for replacing billboards in the videos.
output_videos/ - Contains the processed videos with the replaced advertisement.
Files
Ad Replacement Code: The core code that performs the following tasks:

Loads a YOLO model to detect the billboard area in the video.
Processes each video frame and dynamically replaces the detected billboard with the ad image.
Handles challenges such as camera movement, lighting adjustments, and angle variations for seamless ad placement.
Ad Image: The advertisement image that will be used to replace billboards in the video content. This image can be customized to fit different ad campaigns.

Output Videos: These are the processed videos where the billboard has been replaced by the specified ad image.

Key Features
YOLOv8 for Billboard Detection: The code uses YOLOv8 to detect billboard areas in the video and dynamically adjust the ad's size, perspective, and lighting to ensure it looks natural.
Seamless Ad Placement: The ad is resized and transformed to fit the detected billboard area, with additional lighting adjustments for blending the ad smoothly into the frame.
Support for Camera Movement: By detecting the billboard in each frame, the program ensures that the ad stays correctly positioned even if the camera moves or the billboard's appearance changes.
Running the Program
To run the program, follow these steps:

Ensure you have the necessary dependencies installed (OpenCV, YOLO, etc.).
Place your training, testing, and validation data in the corresponding folders (train/, test/, valid/).
Place the advertisement image you want to use in the ad_image/ folder.
Run the code, and the output videos will be saved in the output_videos/ folder with the billboard replaced by your ad image.
Output
The output videos, located in the output_videos/ folder, show the results of the ad replacement process. Each video has been processed to replace the original billboard with the specified advertisement image.

Conclusion
This project demonstrates a solution for automatic ad replacement in video content, leveraging computer vision and object detection techniques to ensure seamless integration of ads into dynamic video footage.
