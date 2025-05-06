# 🎤 Singing Voice Synthesis Using Generative Models

This project explores and compares deep learning techniques for **singing voice synthesis** using the [VocalSet dataset](https://zenodo.org/records/1193957?utm_source=chatgpt.com). Inspired by the [HiddenSinger](
https://doi.org/10.48550/arXiv.2306.06814) paper, the project implements and evaluates four generative models:

- 🎨 **Diffusion Model (DDPM)**
- 🧠 **Generative Adversarial Network (GAN)**
- 🔢 **Vector Quantized Variational Autoencoder with Transformer (VQ-VAE Transformer)**
- 🧼 **Denoising Autoencoder (DAE)**

Each model was trained on labeled human singing data and evaluated based on audio quality, training stability, generation speed, and architectural complexity.

---

## 📁 Project Structure

```bash
Project/
│
├── denoising.ipynb # DAE implementation and spectrogram denoising
├── transformer.ipynb # VQ-VAE with Transformer training and inference
├── gans.ipynb # GAN model for singing synthesis
├── diff_model.ipynb # Latent diffusion-based synthesis
├── report/ # Full LaTeX IEEE-formatted research report
└── README.md # You're here!
```


---

## 🔬 Key Features

- 🎼 Preprocessing of VocalSet dataset (trimming, normalization, spectrograms)
- 📉 Visualizations: loss curves, spectrogram comparisons, waveform plots
- 🔊 Output samples showcasing each model’s generative quality
- 📄 IEEE-style research paper included
- ⚖️ Comparative table of model performance
- 💡 Suggestions for future improvements like DDIM, hybrid models, and conditioning

---

## 🧪 Models at a Glance

| Criterion              | Diffusion | GANs        | VQ-VAE Transformer | DAE                    |
|------------------------|-----------|-------------|--------------------|-------------------------|
| Training Stability     | High      | Low         | Medium             | High                    |
| Inference Speed        | Low       | High        | Medium             | Very High               |
| Output Quality         | Highest   | Medium-High | High               | Low                     |
| Generalization         | High      | Low-Medium  | High               | Low                     |
| Complexity             | High      | Medium      | Very High          | Low                     |
| Best Use Case          | Studio-quality synthesis | Quick FX | Expressive singing | Simple denoising      |

---

---

## 🚀 Getting Started
```bash
git clone https://github.com/Eman-Furrukh/Singing-Voice-Synthesis-Using-Generative-Models.git
cd Singing-Voice-Synthesis-Using-Generative-Models
pip install -r requirements.txt
jupyter notebook
```

## 📝 Paper Reference
This project is inspired by:

HiddenSinger: High-Quality Singing Voice Synthesis via Neural Audio Codec and Latent Diffusion Models
K. Lee, Y. Huh, Y. Lee, J. Kim, J. Nam
International Conference on Learning Representations (ICLR), 2023
arXiv:2303.15406

## 👩‍💻 Authors
Eman Furrukh – @Eman-Furrukh

Shamail Aamir Khan - @shamail-123
