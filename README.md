# Tiger-Pose-Estimation

## **Project Overview**

This project showcases the application of deep learning in pose estimation for tigers using the Ultralytics YOLO-Pose model. The goal is to detect and analyze tiger body keypoints, which can be used in wildlife monitoring, behavior analysis, and conservation.

**Setting Up Colab Environment**
  
  ##### Ensure Colab notebook is configured to use GPU for faster processing.


**Data Structure:**

Images: Annotated tiger images.

Annotations: 12 keypoints per tiger (head, legs, tail, etc.)


The YOLO-Pose model is typically trained for human pose estimation, so to get accurate results for tiger pose estimation,need to retrain or fine-tune the model using the Tiger-Pose dataset.

### YOLO-Pose for tiger pose estimation  
#### Transfer learning Approach

**Model Training**

The YOLO-Pose architecture modifies the standard YOLO object detection framework to output keypoint coordinates (x, y) instead of just bounding boxes.

Instead of classifying entire objects, the model predicts each keypoint’s exact position within the bounding box.

It minimizes errors by optimizing the Euclidean distance between predicted and ground truth keypoints.


