# 🖼️ Image Captioning with LLaMA-3 & CLIP Vision Transformer

This project demonstrates how to build an **image captioning system** by combining **CLIP's Vision Transformer** (for visual feature extraction) with **LLaMA-3** (for language generation).  
The system encodes an image into embeddings using CLIP, maps them into LLaMA’s embedding space, and generates coherent natural-language captions.

---

## 🚀 Overview

- Extracts **visual features** from images using CLIP.
- Uses a **projection layer** to align CLIP embeddings with LLaMA-3’s input space.
- Generates **textual captions** with LLaMA-3’s autoregressive decoding.
- Includes preprocessing, training setup, and evaluation metrics.

---

## ⚙️ Installation

Install the required packages:

```bash
pip install lightning torchmetrics spacy
python -m spacy download en_core_web_sm
