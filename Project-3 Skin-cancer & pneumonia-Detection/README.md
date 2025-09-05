# 🩺 Project 3: Skin Cancer and Pneumonia Detection

## 📌 Objective

This project applies **Deep Learning** techniques to classify medical
images for detecting **Skin Cancer** and **Pneumonia**.\
The main goal is to implement two different models: one using **Transfer
Learning** and another using a **Custom CNN**.

------------------------------------------------------------------------

## 🧪 1. Skin Cancer Detection

-   **Dataset:** Subset of the ISIC Skin Cancer Dataset (≈700 images).\
-   **Preprocessing:** Images resized to 128x128, normalized.\
-   **Model:** ResNet50 (Transfer Learning, pre-trained on ImageNet).\
-   **Loss Function:** Binary Crossentropy.\
-   **Optimizer:** Adam (learning rate 0.0001).\
-   **Evaluation:** Accuracy on validation dataset.

------------------------------------------------------------------------

## 🫁 2. Pneumonia Detection

-   **Dataset:** Subset of the Kaggle Chest X-Ray Dataset (≈700
    images).\
-   **Preprocessing:** Same as Skin Cancer.\
-   **Model:** Simple CNN with 2 convolutional layers.\
-   **Loss Function:** Binary Crossentropy.\
-   **Optimizer:** Adam (learning rate 0.0001).\
-   **Evaluation:** Accuracy + ROC Curve with AUC Score.

------------------------------------------------------------------------

## 📊 Results & Graphs

-   Training and validation accuracy/loss curves are plotted for each
    model.\
-   ROC curve is generated for Pneumonia detection to evaluate
    classification performance.

------------------------------------------------------------------------

## ⚙️ Technologies & Libraries Used

-   **Python**
-   **TensorFlow / Keras**
-   **Scikit-learn**
-   **Matplotlib**
-   **Pillow (PIL)**

------------------------------------------------------------------------

## ✅ Outcome

-   Two trained models were developed:
    -   **Skin Cancer Detection (ResNet50)** → Good accuracy with
        Transfer Learning.\
    -   **Pneumonia Detection (CNN)** → Balanced performance with
        ROC/AUC evaluation.\
-   These models demonstrate the potential of AI in **early disease
    detection** using medical images.
