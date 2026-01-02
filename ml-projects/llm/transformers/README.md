# Transformer-Based Text Classification (SQuAD)

This project demonstrates **fine-tuning and evaluation of pretrained transformer models**
for a **text classification task** using the Hugging Face ecosystem.

The goal is to analyze how different transformer architectures perform in terms of
**classification accuracy and training cost**, rather than to achieve state-of-the-art results.

---

## 📌 Project Overview

- Task: Text classification
- Models: Pretrained transformer architectures (BERT-like)
- Framework: Hugging Face Transformers
- Dataset: Processed subset of SQuAD adapted for classification
- Focus: Model performance vs. computational cost

This is an applied NLP project showing a complete, reproducible workflow:
from data preparation to model evaluation.

---

## 🧠 Problem Formulation

Although the original **SQuAD dataset** is designed for question answering,
it is transformed here into a **classification problem** by constructing
(context, question, label) examples.

This allows transformer models to be evaluated in a supervised classification setting,
highlighting architectural trade-offs rather than dataset-specific performance.

---

## 🔧 Workflow

1. **Data Loading**
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

5. **Comparison**
   - Compare different transformer architectures
   - Analyze trade-offs between model size, accuracy, and efficiency

---

## 🛠 Technologies

- Python
- Hugging Face Transformers
- Hugging Face Datasets
- scikit-learn
- PyTorch
- NumPy

---

## 🎯 Key Takeaways

- Pretrained transformers can be efficiently adapted to classification tasks
- Larger models do not always justify higher computational cost
- Model selection should consider **performance–cost trade-offs**, not accuracy alone

---

## 📂 Files

- `transformer_text_classification.ipynb` – main notebook with training and evaluation pipeline

---

## 🚀 Possible Extensions

- Add cross-model benchmarking with standardized evaluation
- Include memory and inference-time measurements
- Extend to multi-label or multi-task classification
- Integrate results into a broader LLM evaluation framework
