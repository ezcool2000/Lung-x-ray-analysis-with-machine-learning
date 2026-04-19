#  AI-Powered Chest X-Ray Diagnostics (COVID-19 & Pneumonia)

This repository contains a Deep Learning project developed for a Biomedical Engineering Graduation Thesis. The system utilizes Transfer Learning to classify chest X-ray images into four categories: COVID-19, Viral Pneumonia, Lung Opacity, and Normal.

##  Project Overview
Medical imaging classification requires high precision. This project leverages the power of a pre-trained **ResNet50V2** model. By freezing the base layers and fine-tuning the top 50 layers, the model acts as an AI assistant for radiologists, significantly reducing diagnosis time.

* **Dataset:** 33,000+ Chest X-Ray images (Kaggle COVID-19 Radiography Dataset)
* **Architecture:** ResNet50V2 (Transfer Learning + Fine-Tuning)
* **Categories:** 4 Classes (COVID, Lung Opacity, Normal, Viral Pneumonia)

## Performance & Results
The model achieved an overall accuracy of **81%** on a completely unseen test set of 8,466 images.

**Key Highlights from the Confusion Matrix:**
* **Viral Pneumonia Detection:** Exceptional recall rate of **91%**, successfully identifying 454 out of 499 cases.
* **Normal Lungs:** High precision in distinguishing healthy lungs with an **87%** recall rate.
* **Medical Context:** The model occasionally confuses COVID-19 with 'Lung Opacity'. This aligns with real-world radiological challenges, as the "ground-glass opacity" caused by COVID-19 is visually nearly identical to other bacterial opacities on standard X-Rays without PCR testing.

*<img width="942" height="790" alt="matris" src="https://github.com/user-attachments/assets/d13a4383-8d46-4819-88b6-1843e0912653" />
*

## 💻 Live Inference 
You don't need to retrain the model. You can download the pre-trained weights and test it instantly with any X-Ray image.

download the pre trained brain here: https://drive.google.com/file/d/1AikTDxpkQEdBvMWi7NLuqB0zsHODisyq/view?usp=drive_link
 **Run the inference script:** Upload a random X-ray image and the system will output the probability bar chart in seconds.

*<img width="933" height="390" alt="results" src="https://github.com/user-attachments/assets/f7b7e176-cf3f-4c7f-b052-c83bfbc09303" />
*

## 🛠️ Technologies Used
* **TensorFlow & Keras:** Deep Learning pipeline and model architecture.
* **Python:** Core programming language.
* **Matplotlib & Seaborn:** Data visualization and medical evaluation metrics.
* **Google Colab:** Cloud GPU (T4) training environment.
