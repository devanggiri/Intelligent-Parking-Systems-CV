# Intelligent Parking Systems: Optimizing Space Utilization

## Parking Spot Detector

**Overview**

The Parking Spot Detector is a computer vision-based system that identifies and classifies parking spot occupancy in real-time. By leveraging image classification techniques and Connected Components Analysis (CCA), this project provides an efficient solution for monitoring parking space availability.

**Key Features**

* Real-time detection of occupied and available parking spots.
* Binary mask segmentation for structured tracking.
* Optimized performance using frame-wise change detection.
* Classification frequency reduction to enhance efficiency.

**Dataset**

* Video Data: A parking lot video with occupied and empty spots.
* Mask Image: A binary mask marking parking locations.
* Cropped Video: A smaller processed section for testing.

**Implementation**

* Loading Video & Mask: OpenCV reads the parking lot video. A grayscale mask image is loaded to locate parking spots.
* Detecting Parking Spots: Connected Components Analysis (CCA) extracts bounding boxes for each parking spot.
* Classifying Parking Spots: Cropped images of spots are classified as empty or occupied using a trained model.
* Visualization: Green bounding boxes for available spots, Red for occupied spots.
* Performance Optimization: Classification is performed only on frames with detected changes.
* Final Testing: The model is validated on a larger dataset for real-world applicability.

**Technology & Tools**

* Python (OpenCV, NumPy, Torch)
* Deep Learning Classifier
* Connected Components Analysis (CCA)
* Mask Processing
