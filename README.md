# VAE vs GAN: Image Generation Comparison

A comprehensive comparison of Variational Autoencoders (VAE) and Generative Adversarial Networks (GAN) for image generation tasks using CIFAR-10 dataset.

## 🎯 Overview

This project implements and compares two popular generative models:
- **Variational Autoencoder (VAE)** with encoder-decoder architecture
- **Generative Adversarial Network (GAN)** with similarity-based discriminator

The models are trained on CIFAR-10 cats and dogs subset to generate realistic animal images.

## 🏗️ Architecture

### VAE Components
- **Encoder**: Convolutional layers with batch normalization
- **Decoder**: Transposed convolutions for image reconstruction
- **Latent Space**: 100-dimensional continuous representation

### GAN Components
- **Generator**: Deep convolutional network with batch normalization
- **Discriminator**: Siamese-style similarity discriminator with minibatch discrimination
- **Feature Extractor**: Shared convolutional feature extraction

## 🚀 Features

- Custom VAE implementation with KL divergence regularization
- Advanced GAN with similarity-based discrimination
- Minibatch discrimination for diversity promotion
- Comprehensive quantitative evaluation metrics
- Visual comparison of generated samples
- Real-time training loss visualization

## 📊 Results

- **VAE**: Stable training, blurry but structured outputs
- **GAN**: More detailed generations but training instability
- **Performance**: VAE achieves lower MSE (0.0901 vs 0.1919)

## 🛠️ Requirements

```bash
tensorflow>=2.8.0
numpy>=1.21.0
matplotlib>=3.5.0
```

## 💻 Usage

```python
python generative_models_comparison.py
```

The script will:
1. Load and preprocess CIFAR-10 data
2. Train both VAE and GAN models
3. Generate comparison visualizations
4. Output quantitative metrics

## 📈 Evaluation Metrics

- Mean Squared Error (MSE)
- Reconstruction Loss
- KL Divergence
- Similarity Scores
- Visual Quality Assessment

## 🔧 Configuration

Key hyperparameters:
- Batch Size: 64
- Latent Dimension: 100
- Learning Rate: 1e-4
- Training Epochs: 30

## 📝 License

MIT License - feel free to use and modify for your projects.

## 🤝 Contributing

Contributions welcome! Feel free to submit issues and pull requests.
