# Transformer-Based Text Classification (SQuAD)

This project demonstrates **fine-tuning and comparative evaluation of pretrained transformer models**
for a **text classification task** using the Hugging Face ecosystem.

The focus is on understanding **performance–cost trade-offs** between different transformer architectures,
rather than achieving state-of-the-art results on a single model.

---

## 📌 Project Overview

- Task: Text classification
- Models: Pretrained transformer architectures (BERT-like)
- Framework: Hugging Face Transformers
- Dataset: Processed subset of SQuAD adapted for classification
- Focus: Accuracy, training time, and architectural trade-offs

This is an applied NLP project presenting a **complete and reproducible workflow**,
from data preparation and fine-tuning to cross-model comparison.

---

## 🧠 Problem Formulation

Although the original **SQuAD dataset** is designed for question answering,
it is transformed here into a **supervised classification problem** by constructing
(context, question, label) examples.

This formulation allows different transformer architectures to be compared
in a controlled classification setting, independent of QA-specific metrics.

---

## 🔧 Workflow

1. **Data Loading and Preprocessing**
   - Load and preprocess SQuAD-style data
   - Convert hierarchical QA structure into flat classification samples

2. **Tokenization**
   - Use model-specific tokenizers via `AutoTokenizer`
   - Apply truncation and padding for batch processing

3. **Model Fine-Tuning**
   - Initialize pretrained models with `AutoModelForSequenceClassification`
   - Fine-tune using Hugging Face `Trainer`

4. **Evaluation**
   - Measure classification performance (e.g. accuracy)
   - Track training time to assess computational cost

5. **Model Comparison**
   - Compare multiple transformer architectures
   - Analyze trade-offs between model size, accuracy, and efficiency

---

## 📂 Project Files

- `hf_transformer_finetuning_training.ipynb`  
  End-to-end fine-tuning pipeline for transformer-based text classification:
  data preparation, tokenization, training, and basic evaluation.

- `hf_transformer_finetuning_comparison.ipynb`  
  Comparative analysis of different pretrained transformer architectures,
  focusing on classification performance and training cost.

---

## 🛠 Technologies

- Python
- Hugging Face Transformers
- Hugging Face Datasets
- PyTorch
- scikit-learn
- NumPy

---

## 🎯 Key Takeaways

- Pretrained transformer models can be efficiently adapted to classification tasks
- Increased model size does not always justify higher computational cost
- Practical model selection should consider **accuracy, efficiency, and scalability**

---

## 🚀 Possible Extensions

- Add standardized cross-task benchmarking
- Include memory usage and inference-time measurements
- Extend to multi-label or multi-task classification
- Integrate results into a broader LLM evaluation or benchmarking framework
