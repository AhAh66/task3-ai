# Object Recnaztion 

## Overview
This project performs **object Recnaztion** using OpenCV's Deep Neural Network (DNN) module. It utilizes a pre-trained **MobileNet SSD** model to detect and classify objects in an image.

## Requirements
Make sure to install the required dependencies before running the script:
```sh
pip install opencv-python numpy
and files that i upload here
```

## How It Works
1. **Load the image**: Reads an input image (`person.png`).
2. **Load Class Labels**: Reads `coco.names`, which contains the list of object classes.
3. **Load the Model**: Loads the **SSD MobileNet V3** model using TensorFlow pre-trained weights (`frozen_inference_graph.pb`).
4. **Object Recnaztion**:
   - The model processes the image to detect objects.
   - It applies a confidence threshold (default: `0.5`) to filter detections.
5. **Draw Bounding Boxes**:
   - If objects are detected, bounding boxes are drawn around them.
   - Each object is labeled with its **class name** and **confidence score**.
6. **Display the Result**: Shows the output image with detected objects.

## Files Used
The necessary files are included in the project:
- `person.png` → Input image
- `coco.names` → List of object classes
- `ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt` → Model configuration file
- `frozen_inference_graph.pb` → Pre-trained model weights

## Running the Script
Run the script using Python:
```sh
python detect_objects.py
```

## Expected Output
- If objects are detected, they will be highlighted with bounding boxes and labels.
- If no objects are found, the message **"No objects detected."** will be displayed.

## Notes
- Ensure that all necessary files are present in the project directory.


