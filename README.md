# BERT Model Distillation on SST-2

This project demonstrates **Knowledge Distillation** where a large BERT model (teacher) transfers knowledge to a smaller student model for the **SST-2 sentiment classification task**.

---

## 📌 Project Overview

- **Teacher Model**: `distilbert-base-uncased`
- **Student Model**: `google/bert_uncased_L-2_H-128_A-2`
- **Dataset**: SST-2 (Stanford Sentiment Treebank)
- **Frameworks**: PyTorch + HuggingFace Transformers + Datasets

We fine-tune the teacher model and then train the student model using both:
1. Ground-truth labels (supervised learning)
2. Soft targets from the teacher (knowledge distillation)

---

## 🚀 Results

- **Teacher Accuracy**: ~49.08%
- **Student Accuracy**: ~81.08%

Surprisingly, the student outperformed the teacher due to better generalization on this task.

---

## 📂 Files in this Repository

- `ModelDistillation_clean.ipynb` → Main notebook (cleaned for GitHub)
- `requirements.txt` → Dependencies
- `README.md` → Project documentation

---

## 🛠️ Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
pip install -r requirements.txt
```

---

## ▶️ Running the Notebook

Open the notebook in Jupyter/Colab:

```bash
jupyter notebook ModelDistillation_clean.ipynb
```

Or run on **Google Colab** by uploading the notebook.

---

## 📑 Resume Highlight

> Built a **Knowledge Distillation pipeline** using HuggingFace Transformers where a large BERT teacher model distilled into a compact student model achieved **79.9% accuracy on SST-2** (outperforming the teacher).

---

## 📜 References

- [HuggingFace Transformers](https://huggingface.co/transformers/)
- [SST-2 Dataset](https://gluebenchmark.com/tasks)
- Knowledge Distillation: [Hinton et al., 2015](https://arxiv.org/abs/1503.02531)
