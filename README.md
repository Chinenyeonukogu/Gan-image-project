# Exploring Image Generation Using BigGAN

This project demonstrates how to generate realistic images using a pretrained BigGAN model from Hugging Face. 
BigGAN is a powerful class-conditional Generative Adversarial Network (GAN) that can generate high-resolution images from random noise and class labels

## 📌 Introduction
Generative Adversarial Networks (GANs) are a powerful class of deep learning models used to generate realistic images and videos. A GAN consists of two neural networks:
- A **generator**, which creates synthetic data from random noise.
- A **discriminator**, which attempts to distinguish real data from fake data.

Through repeated training and competition, the generator learns to produce outputs that resemble real data — such as photographs, objects, or animals — as seen in the training dataset.
## 🧪 Experiment Summary

For this project, I used the `BigGAN` model from Hugging Face’s `pytorch_pretrained_biggan` library. 
BigGAN is a **class-conditional GAN**, meaning it can generate images based on specific ImageNet class labels.

### Tools Used:
- Python
- Jupyter Notebook
- PyTorch
- Hugging Face BigGAN (pretrained)

### Process:
- Selected a class label: e.g., `963` (Pizza)
- Generated a **128-dimensional latent vector** using `torch.randn(1, 128)`
- Paired the vector with a one-hot encoded class vector
- Passed both into the pretrained BigGAN model to generate synthetic images

📚 Acknowledgments
BigGAN paper (DeepMind)
Hugging Face BigGAN
PyTorch Documentation
