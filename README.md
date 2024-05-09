{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "source": [
        "# Music Genre Classification Using Spectrogram Images with MobileNetV2\n",
        "\n",
        "## Overview\n",
        "This project uses the MobileNetV2 architecture to classify music genres based on spectrogram images. It employs transfer learning to enhance model performance on the GTZAN dataset, which consists of images representing ten different music genres.\n",
        "\n",
        "## Prerequisites\n",
        "Ensure you have the following installed:\n",
        "- Python 3.8 or above\n",
        "- TensorFlow 2.7 or newer\n",
        "- Pandas\n",
        "- NumPy\n",
        "- Matplotlib\n",
        "- Scikit-Learn\n",
        "\n",
        "Install all required packages using the command:\n"
      ],
      "metadata": {
        "id": "GnhnmcnvELpT"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "pip install -r requirements.txt"
      ],
      "metadata": {
        "id": "TXvYUKR_EKyZ"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "\n",
        "## Dataset\n",
        "The dataset is sourced from Kaggle's GTZAN genre collection. The data should be organized in the following directory structure on Google Drive:\n",
        "\n"
      ],
      "metadata": {
        "id": "-BK3fpaHET7n"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "/content/drive/MyDrive/Deep Learning/Data/images_original/\n",
        "|-- blues\n",
        "|-- classical\n",
        "|-- country\n",
        "|-- disco\n",
        "|-- hiphop\n",
        "|-- jazz\n",
        "|-- metal\n",
        "|-- pop\n",
        "|-- reggae\n",
        "|-- rock"
      ],
      "metadata": {
        "id": "xeyNL-sREbSX"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Each genre directory contains spectrogram images corresponding to that genre.\n",
        "\n",
        "## Google Colab Setup\n",
        "If you are using Google Colab, mount your Google Drive to access the dataset:"
      ],
      "metadata": {
        "id": "Rhng3aTME3Nv"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "from google.colab import drive\n",
        "drive.mount('/content/drive')"
      ],
      "metadata": {
        "id": "uzzIEY57E5TX"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Running the Script\n",
        "All the codes are inside the \"Final Assignment - Nelson Krisanto.py\".\n",
        "\n",
        "Run it from the top cells to the bottom."
      ],
      "metadata": {
        "id": "j8t-MAAeFoAu"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Evaluating the Model\n",
        "To evaluate the model's performance, ensure the model weights are correctly loaded, then run the evaluation section included in the script. The performance metrics such as accuracy, precision, recall, and AUC will be printed."
      ],
      "metadata": {
        "id": "RXJsbtieGG58"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "## Visualizations\n",
        "The project includes code to visualize predictions for a batch of images from the validation set. These can help visually assess the model's performance."
      ],
      "metadata": {
        "id": "FhllreEHGSak"
      }
    }
  ]
}
