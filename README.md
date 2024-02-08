# vit-cnn-image-classification

This student project (serving as a semster project from University of Toronto's UTIAS module AER 1515 – Perception for Robotics) aims to asses the robustness between a pre-trained classical _Convolutional Neural Network_ (CNN) and a pre-trained state-of-the-art _Visual Transformer_ (ViT) model from a [Repo](https://github.com/lukemelas/PyTorch-Pretrained-ViT) for a multi-class image classification task of road signs.
That analysis compares the test dataset with undistorted images against the same, but now corrupted images under varying image qualities - both with several different types and levels of image corupptions using the `imagecorruptions` Python package from this [GitHub Repo](https://github.com/bethgelab/imagecorruptions).

By fine-tuning and comparing both DNNs using `PyTorch`, the project aims to provide insights into their classification task performance and _out-of-the-box_ robustness in realistic driving scenarios with emulated different weather conditions and severenesses.

## Usage

- Clone the repo
- Original training dataset can be found and downloaded from [Kaggle](https://www.kaggle.com/datasets/andrewmvd/road-sign-detection) into the `/src` folder
- Install Python workspace using Conda: `conda env create -f environment.yml`
- Activate Conda environment, then run the following Jupyter Notebooks:
  - `src/data_preprocessing.ipynb`
  - `src/image_corruptions.ipynb`
  - `src/transfer_learning_cnn_multiclass.ipynb`
  - `src/transfer_learning_vit_finetune.ipynb`
