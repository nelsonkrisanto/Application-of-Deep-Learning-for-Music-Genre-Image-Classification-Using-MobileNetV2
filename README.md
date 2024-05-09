# Music Genre Classification Using Spectrogram Images with MobileNetV2

## Overview
This project uses the MobileNetV2 architecture to classify music genres based on spectrogram images. It employs transfer learning to enhance model performance on the GTZAN dataset, which consists of images representing ten different music genres.

## Prerequisites
Ensure you have the following installed:
- Python 3.8 or above
- TensorFlow 2.7 or newer
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn

Install all required packages using the command:
```bash
pip install -r requirements.txt
```

## Dataset
The dataset is sourced from Kaggle's GTZAN genre collection. The data should be organized in the following directory structure on Google Drive:
/content/drive/MyDrive/Deep Learning/Data/images_original/
|-- blues
|-- classical
|-- country
|-- disco
|-- hiphop
|-- jazz
|-- metal
|-- pop
|-- reggae
|-- rock
Each genre directory contains spectrogram images corresponding to that genre.

## Google Colab Setup
If you are using Google Colab, mount your Google Drive to access the dataset:
```bash
from google.colab import drive
drive.mount('/content/drive')
```
## Running the Script
All the codes are inside the "Final Assignment - Nelson Krisanto.py".
Run it from the top cells to the bottom.

## Evaluating the Model
To evaluate the model's performance, ensure the model weights are correctly loaded, then run the evaluation section included in the script. The performance metrics such as accuracy, precision, recall, and AUC will be printed.

## Visualizations
The project includes code to visualize predictions for a batch of images from the validation set. These can help visually assess the model's performance.
