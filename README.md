# Image Captioning with LLaMA-3 & CLIP Vision Transformer  

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)  
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org/)  
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  

---

## Project Overview  

This project implements an **Image Captioning system from scratch** using:  

- **CLIP Vision Transformer (ViT)** for **visual feature extraction**  
- **LLaMA-3** as the **language model** to generate captions  

The system learns to describe images by encoding them into embeddings with CLIP, mapping those embeddings into LLaMA’s embedding space, and using LLaMA’s autoregressive capabilities to generate natural language captions.  

---

## Key Features  

- End-to-end **image captioning pipeline** in PyTorch/Lightning  
- **Preprocessing and feature extraction** using CLIP  
- **Projection layer** to align CLIP embeddings (1024-dim) with LLaMA-3 embeddings (4096-dim)  
- **Caption generation** using LLaMA-3’s autoregressive decoding  
- Easy to extend with different datasets, metrics, or model variants  

---

## Installation  

Clone the repository and install dependencies:  

```bash
git clone https://github.com/Soumit0702/Image_Captioning_using_LLAMA_from_scratch.git
cd Image_Captioning_using_LLAMA_from_scratch

pip install lightning torchmetrics spacy
python -m spacy download en_core_web_sm
