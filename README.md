# Face Mask Detection System

A Computer Vision project that detects whether a person is wearing a face mask or not using OpenCV.

## What it does
- Detects faces in an image using a pre-trained deep learning model
- Classifies each face as Mask or No Mask
- Draws colored bounding boxes (Green = Mask, Red = No Mask)
- Shows detection summary with mask compliance rate

## How to Run
1. Open `face_detection.ipynb` in Google Colab
2. Run all cells from top to bottom
3. Upload any image when prompted
4. See the detection results

## Requirements
All libraries are installed automatically in the notebook:
- OpenCV
- NumPy
- Matplotlib

## How it Works
1. Image is passed through a pre-trained SSD face detector using OpenCV DNN
2. Each detected face region is extracted
3. HSV color thresholding is applied to the lower half of the face
4. If skin ratio is low, mask is detected. Otherwise, no mask.

## Limitations
- Dark colored masks may not be detected accurately
- Works on static images only
- Performance may vary with lighting and face angles

## Tech Stack
- Python
- OpenCV
- Google Colab
