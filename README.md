# Adversarial Attacks on Traffic Sign Classification

This project explores the vulnerability of deep learning models to various adversarial attacks. Using a **ResNet-34** model trained on a traffic sign dataset, I demonstrate how small, carefully crafted perturbations can drastically affect model predictions, despite high accuracy on clean data.

## 📌 Project Overview

I implement and analyze several adversarial attack techniques:

- **FGSM (Fast Gradient Sign Method)**
- **PGD (Projected Gradient Descent)**
- **DeepFool**
- **Carlini & Wagner (C&W)**
- **Adversarial Patch Attack**

I also explore:

- The effect of random perturbations (noise and JPEG compression) vs. adversarial changes
- The robustness of the model to black patches versus adversarial patches

The goal is to highlight the difference between unintentional and adversarial perturbations, and to demonstrate the effectiveness of targeted attacks against neural networks in safety-critical applications like traffic sign recognition.

## 🧪 Features

- Evaluate model performance on clean and adversarial images
- Compare subtle (FGSM, PGD) and visible (patch) attacks
- Demonstrate model robustness to benign distortions
- Visualize predictions and attack effects

## 🖼️ Model

The model used is a **ResNet-34** trained to classify various traffic signs. It achieves high accuracy on clean test data and serves as a baseline to evaluate how different adversarial methods can break its reliability.

---

## 🛠 Installation

This project uses **[Poetry](https://python-poetry.org/)** for dependency management and **[pyenv](https://github.com/pyenv/pyenv)** for managing Python versions.

### Install Python via Pyenv

Make sure `pyenv` is installed, then run:

```bash
pyenv install 3.12.9
pyenv local 3.12.9
poetry shell
poetry install
```
