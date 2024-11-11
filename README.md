# Monetico: An Efficient Reproduction of Meissonic for Text-to-Image Synthesis

<div align="center">

[![arXiv](https://img.shields.io/badge/arXiv-2410.08261-b31b1b.svg)](https://arxiv.org/abs/2410.08261)
[![Hugging Face](https://img.shields.io/badge/🤗%20Huggingface-Model-yellow)](https://huggingface.co/Collov-Labs/Monetico)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-181717?logo=github)](https://github.com/collovlabs/Monetico)

</div>


## 🚀 Introduction

Similar to Meissonic, Monetico is a non-autoregressive masked image modeling text-to-image synthesis model capable of generating high-resolution images. It is designed to run efficiently on consumer-grade graphics cards.

Monetico is an efficient reproduction of Meissonic. Trained on 8 H100 GPUs for approximately one week, Monetico can generate high-quality 512x512 images that are comparable to those produced by Meissonic and SDXL.

Monetico was developed by Collov Labs. We extend our gratitude to @MeissonFlow and @viiika for their valuable advice on efficient training.

## 🛠️ Prerequisites

### Step 1: Clone the repository
```bash
git clone https://github.com/collovlabs/Monetico/
cd Monetico
```

### Step 2: Create virtual environment
```bash
conda create --name monetico python
conda activate monetico
pip install -r requirements.txt
```

### Step 3: Install diffusers
```bash
git clone https://github.com/huggingface/diffusers.git
cd diffusers
pip install -e .
```

## 💡 Usage

### Gradio Web UI

```bash
python app_Monetico.py
```

### Command-line Interface

#### Text-to-Image Generation

```bash
python inference_fp16_Monetico.py --prompt "Your creative prompt here"
```

## 📚 Citation

If you find this work helpful, please consider citing:

```bibtex
@article{bai2024meissonic,
  title={Meissonic: Revitalizing Masked Generative Transformers for Efficient High-Resolution Text-to-Image Synthesis},
  author={Bai, Jinbin and Ye, Tian and Chow, Wei and Song, Enxin and Chen, Qing-Guo and Li, Xiangtai and Dong, Zhen and Zhu, Lei and Yan, Shuicheng},
  journal={arXiv preprint arXiv:2410.08261},
  year={2024}
}
```

<p align="center">
  Made with ❤️ by the Collov AI
</p>
