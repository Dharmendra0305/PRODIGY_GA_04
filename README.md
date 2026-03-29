# Image-to-Image Translation with cGAN 🌍🗺️

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org)
[![Gradio](https://img.shields.io/badge/Gradio-Web%20App-ff69b4.svg)](https://gradio.app)
[![Prodigy InfoTech](https://img.shields.io/badge/Internship-Prodigy%20InfoTech-purple.svg)](#)

## 📌 Overview
This project implements an Image-to-Image translation model using a **Conditional Generative Adversarial Network (cGAN)**, specifically the **Pix2Pix** architecture. It is designed to synthesise map layouts directly from aerial satellite imagery. 

*Here’s the main interface of the Image-to-Image Translation with cGAN:*

![img]()

This repository serves as **Task 04** for my Data Science/Machine Learning Internship at **Prodigy InfoTech**, demonstrating practical skills in advanced deep learning, computer vision, and interactive model deployment.

## ✨ Features
* **U-Net Generator:** Utilises skip connections to preserve high-resolution details during image translation.
* **PatchGAN Discriminator:** Evaluates images at the patch level to enforce high-frequency sharpness and realistic textures.
* **Custom Training Loop:** Implements adversarial loss combined with L1 loss to ensure structural accuracy.
* **Interactive Web UI:** Includes a deployed Gradio application allowing users to upload their own satellite images and generate maps in real-time.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Deep Learning Framework:** TensorFlow 2.x / Keras
* **Deployment/UI:** Gradio
* **Data Manipulation & Visualization:** NumPy, Matplotlib

## 🚀 Installation & Setup

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Dharmendra0305/PRODIGY_GA_04.git](https://github.com/Dharmendra0305/PRODIGY_GA_04.git)

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. **Install the required dependencies:**
   ```bash
   pip install tensorflow numpy matplotlib gradio

## 💻 Usage
- Training the Model
  If you want to train the model from scratch, you can run the provided Jupyter/Colab notebook (Pix2Pix_Training.ipynb). It includes the code to download the
  dataset, build the architecture, and execute the training loop.

- Running the Web App
  *(Ensure you save the Python code provided previously into a file named app.py)*
  To launch the interactive Gradio interface using the pre-trained model:
  ```bash
  python app.py

This will generate a local URL (e.g., http://127.0.0.1:7860/) where you can upload satellite images and see the generated map results.

![img]()

## 🤝 Contribution Guidelines
- Contributions, issues, and feature requests are welcome!
  1. Fork the project.
  2. Create your feature branch (git checkout -b feature/AmazingFeature).
  3. Commit your changes (git commit -m 'Add some AmazingFeature').
  4. Push to the branch (git push origin feature/AmazingFeature).
  5. Open a Pull Request.

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
