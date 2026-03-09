# Gender Classification CNN
Automatic gender detection (male/female) from face images using Transfer Learning with MobileNetV2.

This project uses a Deep Learning model based on pretrained MobileNetV2 to classify a person's gender from a photo of their face.
It supports classification of static images as well as real-time detection via the Google Colab camera.

## Why Transfer Learning ?
The dataset contains only 220 training images.
MobileNetV2, already trained on millions of images (ImageNet),
allows good performance even with limited data.

## Dataset
Source : [Gender Detection & Classification](https://www.kaggle.com/datasets/trainingdatapro/gender-detection-and-classification-image-dataset)
Structure:
Gender/
  ├── train/
  │   ├── men/      # 110 images
  │   └── women/    # 110 images
  └── validation/
      ├── men/      # 40 images
      └── women/    # 40 images

Total : 300 images (220 train / 80 validation)
Classes : Balanced 50% male / 50% female

## Dependencies

- Python
- TensorFlow / Keras
- NumPy
- OpenCV
- Matplotlib
- Google Colab

## Results

The model was trained using the Adam optimizer with a learning rate of 0.0001 and Binary Crossentropy as the loss function.
Training ran for up to 30 epochs with Early Stopping enabled to prevent overfitting.
All input images were resized to 150x150 pixels before being fed into the model.

## Running the Project

1. Clone the repository
bash
```
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. Install dependencies
bash
```
pip install tensorflow numpy opencv-python Pillow matplotlib
```

3. Download the dataset
Download the dataset from Kaggle and place it in your Google Drive :

4. Open in Google Colab
Upload the notebook to Google Colab, mount your Google Drive and run all cells.



## Author

Faiza CS
