# 🧠 Pix2Pix GAN – Satellite to Map Translation

This project uses a **Pix2Pix GAN** model to translate building outline images to real facade images using the **CMP Facades dataset**.

## 📁 Dataset
- Dataset: [`cycle_gan/facades`](https://www.tensorflow.org/datasets/catalog/cycle_gan#cycle_ganfacades)
- Loaded via `tensorflow_datasets`
- Preprocessed, resized to 256×256, normalized to [-1, 1]

## 🧠 Model Details
- Generator: U-Net
- Discriminator: PatchGAN
- Loss: Binary Crossentropy + L1 loss

## 🔁 Training
- Trained on 100 samples × 5 epochs for demo purposes
- Optimizer: Adam (lr=2e-4, β1=0.5)

## 📊 Sample Output

| Input | Target | Predicted |
|-------|--------|-----------|
| ![sample output](sample_output.png) |

_(Screenshot of Input → Target → Predicted image)_

## 📦 Libraries Used
- TensorFlow
- TensorFlow Datasets
- TensorFlow Examples (for `pix2pix`)
- Matplotlib



