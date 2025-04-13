# 🧠 MNIST Digit Synthesis using GANs (PyTorch)

## 📘 Project Overview

This project demonstrates how to generate handwritten digit images using a **Generative Adversarial Network (GAN)** trained on the **MNIST dataset**. Implemented in **PyTorch**, this project showcases the power of adversarial training for generating realistic images of digits (0–9).

---

## 🎯 Objectives

- Understand the fundamentals of GAN architecture
- Implement a simple GAN from scratch using PyTorch
- Train the GAN on the MNIST dataset
- Generate and visualize synthetic digit images
- Track generator and discriminator performance across training epochs

---

## 🧰 Tools and Libraries

- Python
- PyTorch
- torchvision
- matplotlib
- numpy

---

## 🧱 Architecture

### Generator
- Takes random noise (`z`) as input (usually sampled from a normal distribution)
- Uses transposed convolutional layers to generate 28x28 grayscale digit-like images
- Trained to "fool" the discriminator

### Discriminator
- A binary classifier that distinguishes between real and fake digit images
- Trained to correctly identify real MNIST images and reject synthetic ones

> The two models are trained simultaneously in an adversarial loop:  
> The Generator tries to make the Discriminator fail, while the Discriminator tries to improve its classification.

---

## 🏋️ Training Details

- **Dataset**: MNIST (28x28 grayscale images of digits)
- **Epochs**: 100
- **Batch Size**: 128 (configurable)
- **Loss Function**: Binary Cross Entropy (BCE)
- **Optimizer**: Adam

---

## 📈 Evaluation Strategy

- Real-time visualization of generated samples during training
- Plotting **Generator Loss** vs **Discriminator Loss** to monitor stability
- Optional: visual exploration of latent space with fixed noise vectors

---

## 🖼️ Generated Samples

Below are the generated digits at various training stages (save and commit your images into the `outputs/` folder):

### 🔢 Epoch 1
![Epoch 1](/Screenshot 2025-04-13 234610.png)

### 🔢 Epoch 20
![Epoch 20](outputs/epoch_020.png)

### 🔢 Epoch 50
![Epoch 50](outputs/epoch_050.png)

### 🔢 Epoch 100
![Epoch 100](outputs/epoch_100.png)

---

## 🧠 Outcome

By the end of training, the generator learns to produce high-quality handwritten digits that closely resemble real MNIST images. The results demonstrate the potential of GANs for image synthesis and open the door to more advanced generative techniques.

---

---

## 💡 Future Extensions

- Conditional GANs (CGANs) to generate digits based on class labels
- Deep Convolutional GAN (DCGAN) architecture
- Explore different loss functions (e.g., Wasserstein GAN)
- Implement image interpolation across the latent space

---

## 🤝 Credits

This project is developed as a hands-on introduction to GANs and PyTorch. It provides a stepping stone for diving deeper into generative models.

---

## 📜 License

This project is open-source and available for educational and research purposes.



