# Image_Background_Remove
This notebook, BG_Remove.ipynb, demonstrates the process of removing the background from images using **Mask R-CNN** algorithm. The model leverages modern computer vision algorithms to detect and extract the foreground objects, while eliminating the background, which is useful for tasks like object segmentation, product photo editing, or artistic design.
## Key Features
**Image Preprocessing**: For reading and writing the images, OpenCV library is used here. pscaling technique is used for converting all images into same heights and widths.
**Model Architecture**: Detectron2's Mask R-CNN model is used for instance segmentation. The model is pre-trained on the COCO dataset. The device is set to either GPU or CPU depending on availability.
**Segmentation Masks**: Once the model detects the objects in the image, it outputs segmentation masks, which are used to identify the object of interest.
**Mask Application**: The mask is applied to the image to isolate the object, removing the background around the detected object.
## Dataset
The image dataset is retrieved from https://www.kaggle.com/datasets/mexwell/locbeef-beef-quality-image-dataset
## Requirements
  1. Python 3.12
  2. PyTorch
  3. OpenCV
  4. NumPy
  5. Matplotlib
## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.
## License
This project is licensed under the Apache 2.0 License - see the LICENSE file for details.
