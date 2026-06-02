# 📄 Fine-Tuning Qwen2-VL for Mathematical OCR

## Overview

This project fine-tunes the **Qwen2-VL-7B Vision Language Model** to perform **Optical Character Recognition (OCR) for mathematical expressions**, generating accurate **LaTeX representations** directly from equation images.

The model is trained using **LoRA (Low-Rank Adaptation)** and **4-bit quantization** through the **Unsloth** framework, enabling memory-efficient fine-tuning while maintaining strong performance.

---

## 🚀 Features

* Convert mathematical equation images into LaTeX code
* Fine-tune Qwen2-VL-7B using LoRA
* Memory-efficient 4-bit quantized training
* Parameter-Efficient Fine-Tuning (PEFT)
* Accelerated training with Unsloth
* Support for vision-language understanding tasks

---

## 🛠️ Tech Stack

* Python
* PyTorch
* Transformers
* Unsloth
* PEFT (LoRA)
* TRL
* Hugging Face Datasets
* Qwen2-VL-7B

---

## 📚 Dataset

The model is trained on a LaTeX OCR dataset containing:

* Mathematical expression images
* Corresponding LaTeX annotations

This enables the model to learn image-to-LaTeX generation for mathematical OCR tasks.

---

## ⚙️ Training Pipeline

1. Load Qwen2-VL-7B Vision Language Model
2. Apply 4-bit quantization for memory optimization
3. Configure LoRA adapters for efficient fine-tuning
4. Preprocess dataset into conversational format
5. Fine-tune using SFTTrainer
6. Evaluate model predictions on mathematical expressions

---

## 📂 Project Structure

```text
.
├── finetuning_qwen_vl.ipynb
├── README.md
└── requirements.txt
```

---

## 🔧 Installation

```bash
pip install transformers
pip install datasets
pip install peft
pip install trl
pip install unsloth
```

Or install all dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Launch the notebook:

```bash
jupyter notebook finetuning_qwen_vl.ipynb
```

The notebook covers:

* Dataset preparation
* Model loading
* LoRA configuration
* Fine-tuning
* Inference

---

## 📈 Example

### Input

Image containing a mathematical equation:

```text
∫ x² dx
```

### Output

```latex
\int x^2 \, dx
```

---

## 🎯 Key Learning Outcomes

* Fine-tuning Vision Language Models (VLMs)
* Parameter-Efficient Fine-Tuning (PEFT)
* LoRA-based adaptation
* Quantized model training
* Mathematical OCR systems
* Hugging Face ecosystem workflows

---

## 🔮 Future Improvements

* Evaluate using BLEU and Exact Match metrics
* Support handwritten mathematical expressions
* Train on larger OCR datasets
* Deploy as a web application
* Integrate with document digitization pipelines

---

## 👨‍💻 Author

**Vinit Khapekar**

B.Tech Computer Science Engineering (AI/ML)

## Acknowledgements

This project was recreated and adapted as a learning exercise based on the tutorial by Shreemanti Dey on fine-tuning Vision Language Models using Qwen2-VL and Unsloth.

The implementation was reproduced for educational purposes to understand VLM fine-tuning, LoRA, quantization, and image-to-LaTeX generation workflows.

Interests: LLMs, AI Agents, RAG Systems, Computer Vision, Generative AI, and Machine Learning.
