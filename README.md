# Object detection

## Overview

This project demonstrates an end-to-end object detection pipeline, including data preprocessing, annotation conversion, and model training using YOLOv11. The workflow covers:
- Image resizing and padding to a standard size (640x640)
- Conversion of PASCAL VOC annotations to YOLO format
- Training and inference using the YOLOv11 model

## Features

- Preprocesses images from multiple weather conditions (Rain, Sand, Fog, Snow)
- Converts annotation formats for compatibility with YOLO
- Visualizes original and preprocessed images
- Trains and evaluates object detection models using YOLOv11

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- PyTorch
- ultralytics (for YOLOv11)

Install dependencies with:
```bash
pip install opencv-python numpy matplotlib torch ultralytics
```

## Data Structure

- `./data/`: Contains subfolders for each weather condition (Rain, Sand, Fog, Snow)
- Each subfolder contains images and annotation files in PASCAL VOC format

## Usage

1. **Preprocess Images and Convert Annotations**
   - The notebook resizes images to 640x640 and converts PASCAL VOC annotations to YOLO format for each weather condition.

2. **Visualize Preprocessing**
   - The notebook provides functions to display original and preprocessed images side by side.

3. **Train YOLOv11**
   - The notebook demonstrates how to load and train a YOLOv11 model using the preprocessed data.

## Example

To preprocess images and convert annotations, run the notebook cells under "Data preprocessing -resizing".  
To train the model, follow the cells under "Training using YOLOv11".

## Customization

- Update the `classes` list in the notebook to match your dataset classes.
- Adjust dataset paths as needed.

## Acknowledgements

- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
- OpenCV, PyTorch, and other open-source libraries
