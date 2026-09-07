# 🥦 Vegetable Image Classifier

Deep learning project that classifies images into 15 vegetable categories (Bean, Bitter Gourd, Bottle Gourd, Brinjal, Broccoli, Cabbage, Capsicum, Carrot, Cauliflower, Cucumber, Papaya, Potato, Pumpkin, Radish, Tomato).

Trained on the [Vegetable Image Dataset](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset) using three architectures for comparison:
- A custom CNN built from scratch
- **MobileNetV2** (transfer learning, ImageNet weights)
- **EfficientNetB0** (transfer learning, ImageNet weights)

The best-performing model is served through a simple **Streamlit** app for live image predictions, tunneled with **ngrok** for public access from Google Colab.

## Tech Stack
- TensorFlow / Keras
- Streamlit
- Google Colab + Google Drive (model checkpointing)
- Kaggle API (dataset download)

## How it Works
1. Downloads the dataset via the Kaggle API
2. Trains/loads three models with image augmentation
3. Saves trained models to Google Drive
4. Runs a Streamlit web app where users upload a vegetable image and get a predicted class


