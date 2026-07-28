<img width="416" height="332" alt="Screenshot 2026-07-26 234405" src="https://github.com/user-attachments/assets/ef9b56c6-9294-4d58-addf-6f6d7d2dcdcc" />
# Fine-Tuning Llama 3.2 3B with QLoRA

This project demonstrates how to efficiently fine-tune Meta's **Llama 3.2 3B** model using **QLoRA (Quantized Low-Rank Adaptation)** for a domain-specific next-token prediction task.

The project covers the complete fine-tuning workflow, from dataset preparation to training, evaluation, and publishing the fine-tuned model on Hugging Face.

## 🚀 Features

- Fine-tuning Meta Llama 3.2 3B
- QLoRA (4-bit Quantization)
- PEFT (Parameter Efficient Fine-Tuning)
- LoRA Adapters
- Hugging Face TRL SFTTrainer
- Weights & Biases experiment tracking
- Automatic model checkpointing
- Push trained model directly to Hugging Face Hub

## 🛠️ Tech Stack

- Python
- PyTorch
- Transformers
- TRL
- PEFT
- BitsAndBytes
- Accelerate
- Datasets
- Hugging Face Hub
- Weights & Biases

## Fine-Tuning Pipeline

```
Dataset
    │
    ▼
Tokenizer
    │
    ▼
Llama 3.2 3B (4-bit Quantized)
    │
    ▼
LoRA Adapters
    │
    ▼
Supervised Fine-Tuning (SFTTrainer)
    │
    ▼
Cross Entropy Loss
    │
    ▼
Updated LoRA Weights
    │
    ▼
Push to Hugging Face Hub
```

## QLoRA Configuration

- Base Model: Llama 3.2 3B
- Quantization: 4-bit (NF4)
- LoRA Rank (r)
- LoRA Alpha
- LoRA Dropout
- PEFT Training
- BF16/FP16 Training Support

## What I Learned

- Large Language Model Fine-Tuning
- QLoRA Architecture
- LoRA Adapters
- 4-bit Quantization
- Parameter Efficient Fine-Tuning (PEFT)
- Cross Entropy Loss
- Hugging Face TRL
- SFTTrainer
- Model Checkpointing
- Experiment Tracking using Weights & Biases
- Publishing models on Hugging Face

## Results

Successfully fine-tuned a Llama 3.2 3B model using QLoRA while training only the LoRA adapter weights, significantly reducing GPU memory requirements compared to full fine-tuning.

## Future Improvements

- Hyperparameter tuning
- Multi-epoch training
- Larger datasets
- Model evaluation benchmarks
- Inference API deployment

## Author

**Ayush Kashyap**

GitHub: https://github.com/Ayushtechera
