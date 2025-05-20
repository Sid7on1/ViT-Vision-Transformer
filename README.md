# *****ViT-Vision-Transformer*****
ViT-ClassiPy is a lightweight Vision Transformer built from scratch using PyTorch for image classification on datasets like CIFAR-10. It demonstrates patch embedding, positional encoding, transformer blocks, and a custom training loop—ideal for learning transformer-based vision models.

# ViT-ClassiPy

**ViT-ClassiPy** is a minimal Vision Transformer (ViT) implementation built from scratch using PyTorch. Designed for image classification tasks like CIFAR-10, this project demonstrates core transformer components applied to vision, including patch embedding, positional encoding, multi-head attention, and transformer encoders.

---

## 🚀 Features

- Vision Transformer architecture from scratch
- Custom patch embedding and positional encoding
- Multi-head self-attention and MLP blocks
- [CLS] token for classification
- Clean, modular PyTorch code
- Works on CIFAR-10 (easily extensible)

---

## 🧠 Architecture Overview

1. **Patch Embedding** – Split image into fixed-size patches and flatten
2. **Linear Projection** – Embed patches into a vector space
3. **Positional Encoding** – Add spatial information
4. **Transformer Encoder Blocks** – Self-attention + feedforward layers
5. **Classification Head** – Uses [CLS] token for final output

---

## 📊 Dataset

- **Default**: [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)
- **Image size**: 32x32
- **Patch size**: 4x4 (64 patches per image)
- Easily modifiable for other datasets

---

## 🛠️ Installation

```bash
git clone https://github.com/yourusername/vit-classipy.git
cd vit-classipy
pip install -r requirements.txt
```

🏁 Usage
```bash
python train.py
```
This will:
	•	Download the CIFAR-10 dataset
	•	Train the ViT model
	•	Print training and test accuracy

🔧 Configuration

All hyperparameters are defined in config.py:
```bash
IMG_SIZE = 32
PATCH_SIZE = 4
NUM_CLASSES = 10
EMBED_DIM = 128
NUM_HEADS = 4
DEPTH = 6
MLP_DIM = 256
```

📈 Results
Model Dataset Accuracy
ViT-ClassiPy CIFAR-10 ~78%

📌 Note: Accuracy depends on training time and hyperparameters. You can improve it with data augmentation, weight decay, or deeper models.

📌 To-Do
	•	Add attention map visualizations
	•	Add support for custom datasets
	•	Add training logs and checkpoints

📄 License

This project is licensed under the MIT License.

🤝 Contributing

Contributions, ideas, and suggestions are welcome! Feel free to fork the repo and open a pull request.

🙌 Acknowledgements

Inspired by the original ViT paper by Dosovitskiy et al.
