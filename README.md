# Animal Detection using YOLOv5

This repository contains the implementation for animal detection using YOLOv5. The YOLOv5 model is trained, tested, and validated using the provided scripts and folders.

## Files:

1. **train.py**: This script is used for training the YOLOv5 model on the dataset.

2. **test.py**: Use this script to test the trained YOLOv5 model on a test dataset.

3. **val.py**: The validation script evaluates the performance of the model on a validation dataset.

4. **detect.py**: This script is for detecting animals in new images using the trained YOLOv5 model.

## Folders:

1. **runs**: This folder contains the output generated during training and testing.

    - **train**: Output from the training process, including logs, model checkpoints, and training metrics.

    - **detect**: Output from the detection process, including detected bounding boxes and confidence scores.

2. **images_of_performance_metrics**: This folder contains images visualizing the performance metrics obtained during training and testing.

## Usage:

1. Clone the repository:

    ```
    git clone https://github.com/ragulmuthu03/Animal-Detection-Using-YOLOv5
    cd animal-detection-yolov5
    ```

2. Train the model:

    ```
    python train.py --data coco.yaml --epochs 100 --weights yolov5n.pt --cfg yolov5n.yaml  --batch-size 2
    ```

3. Test the model:

    ```
    python test.py --options
    ```

4. Detect animals in new images:

    ```
    python detect.py --weights best.pt --img 416 --conf 0.25 --source 0
    ```

Note: Make sure to customize the options according to your dataset and requirements.

Feel free to explore and contribute to this animal detection project using YOLOv5!
