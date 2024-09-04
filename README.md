# IDEFICS2 Fine-Tuning and Inference

## Project Overview

This project demonstrates fine-tuning and inference with the IDEFICS2 multimodal model on the MathVista dataset.

## Key Features

- Fine-tunes IDEFICS2 on mathematical visual question-answering tasks
- Implements LoRA/QLoRA for efficient model adaptation
- Utilizes Hugging Face Transformers and PEFT libraries
- Incorporates memory optimization techniques:
  - Gradient checkpointing
  - Mixed precision training (FP16)
  - Small batch size with gradient accumulation
- Showcases inference with the fine-tuned model
- Handles both text and image inputs for multimodal processing

## Technologies

- PyTorch
- Hugging Face Transformers
- PEFT (Parameter-Efficient Fine-Tuning)
- Datasets library

## Setup and Usage

[Include instructions for setting up the environment and running the code]

## Model Architecture

- Base model: IDEFICS2 8B
- Fine-tuning method: LoRA/QLoRA
- Target modules: Text model, modality projection, perceiver resampler, attention layers, and feed-forward networks

## Dataset

- Name: MathVista
- Type: Mathematical visual question-answering

## Training Configuration

- Epochs: 1
- Batch size: 1 (with gradient accumulation)
- Learning rate: 1e-4
- Weight decay: 0.01
- Gradient accumulation steps: 16
- Max training steps: 100

## Inference

The script includes an example of running inference with the fine-tuned model on a sample from the test set.
