
# Civic Bot (Qwen2-1.5 – v2)

Civic Bot is a fine-tuned **Qwen2-1.5** language model built to extract **office names and locations** from unstructured text describing government offices. It converts messy, real-world office descriptions into standardized **structured JSON**, making the data easier to store, search, and analyze.

## Key Features

* **Efficient fine-tuning pipeline** using **Unsloth** for fast training and low compute overhead
* **Alpaca-style prompting format** for consistent training and inference behavior
* **Data preparation utilities** for loading, cleaning, tokenizing, and formatting training examples
* **InferenceEngine wrapper** for robust extraction, including fallback handling for incomplete outputs
* **Hugging Face Hub support** to push the fine-tuned model and tokenizer for reuse and deployment

## Model

Base model: **Qwen2-1.5**
Fine-tuned task: structured extraction of **office names + locations** from natural language office descriptions.

## Usage

This notebook demonstrates the full workflow: dependency setup, dataset preparation, fine-tuning, and inference. For extraction on new inputs, the included `InferenceEngine` can be used to generate structured JSON output from raw office descriptions.

---
