# PyFlows

## Using fine-tuned Mistral and DeepSeek models to detect flaws in Python code and produce refactored versions of the code.

## Requirements

To run the provided inference programs locally, you need:

- Python 3.10+
- An NVIDIA GPU with CUDA support
- A GPU compatible with `bfloat16`
- PyTorch 2.2.2
- The Python dependencies listed in [`requirements.txt`](requirements.txt)

### Installation

Install the required Python packages with:

```bash
pip install -r requirements.txt
```

The programs use Hugging Face Transformers and PEFT to load the Mistral or DeepSeek-Coder models and their fine-tuned adapters.

> **Note:** Running the models locally requires sufficient GPU memory. The required GPU memory depends on whether you use the full model or the LoRA adapter version.

## Available Programs

The repository provides inference programs for:

- **Python** code analysis and refactoring
- **Mistral-based** and **DeepSeek-Coder-based** fine-tuned models
- **LoRA adapter** and **full-model** inference

For the LoRA versions, the base model is downloaded automatically from Hugging Face, and the corresponding fine-tuned adapter is loaded.

For the full-model versions, the fine-tuned model is loaded directly from Hugging Face.

## Gradio Interface

For users who prefer a graphical interface, a Gradio-based interface is also available in the related GitHub repository, [Code-Analyzer](https://github.com/Hanan-Abdulwahab-Siala/CodeAnalyzer).

---
