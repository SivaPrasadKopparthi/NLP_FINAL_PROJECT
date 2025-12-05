# 🏥 **HealthInsight: Medical Report Processing Using Transformer Models**

HealthInsight is an AI-powered Natural Language Processing (NLP) system designed to simplify and analyze complex medical reports. The project uses multiple transformer-based models to perform **summarization**, **named entity recognition (NER)**, **similar case retrieval**, and **question–answering (QA)** from medical text.

This system helps convert long, complex medical documents into **clear, meaningful, and structured insights** for doctors, researchers, and patients.

---

## 🚀 **Features**

### 🔹 **1. Summarization**

Models Used:

* **T5-small (Text-to-Text Transfer Transformer – Small)**
* **FLAN-T5-base (Fine-tuned Language Net – T5 Base)**

Purpose:
Generate concise, readable summaries from long medical documents.

### 🔹 **2. Named Entity Recognition (NER)**

Model Used:

* **Biomedical NER Model (Based on BERT – Bidirectional Encoder Representations from Transformers)**

Purpose:
Identify medical entities such as diseases, symptoms, medications, anatomical parts, and treatments.

### 🔹 **3. Similar Case Retrieval**

Model Used:

* **MiniLM Sentence Embedding Model (Miniature Language Model)**

Purpose:
Convert text into embeddings and retrieve medical cases with similar meaning.

### 🔹 **4. Question–Answering (QA)**

Model Used:

* **RoBERTa-based QA Model (Robustly Optimized BERT Approach)**

Purpose:
Answer user questions by extracting relevant information from the medical report.

---

## 📊 **Evaluation Metrics**

We evaluate model performance using:

### ✔ Summarization Metrics

* **ROUGE-1** – matches of single words
* **ROUGE-2** – matches of word pairs
* **ROUGE-L** – longest matching sequence
* **BLEU** – phrase-level precision between reference and generated summary

### ✔ Additional Performance Metrics

* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**

These metrics ensure the generated summaries and predictions align closely with human-written references.

---

## 🧠 **How It Works (Pipeline)**

1. User uploads a medical report (PDF/TXT).
2. Text is extracted and preprocessed.
3. Summarization model generates a short summary.
4. NER model highlights key medical entities.
5. Sentence Embedding model finds similar medical cases.
6. QA model answers user questions about the report.
7. Output is displayed through a **Gradio interface**.

---

## 📦 **Installation**

```bash
git clone <your-repo-url>
cd <your-project-folder>
pip install -r requirements.txt
```

---

## ▶️ **Run the Application**

```bash
python main.py
```

Or open the included **Google Colab notebook** and run all cells.

---

## 📘 **Dataset**

* **PubMed Summarization Dataset**
* Additional sample reports provided by the user

This ensures accurate evaluation in biomedical settings.

---

## 🧪 **Results Summary**

Comparing **T5-small** vs **FLAN-T5-base**, we found:

* **T5-small performed better** in ROUGE-1, ROUGE-L, and BLEU
* **FLAN-T5-base slightly better** in ROUGE-2
* **Accuracy, Precision, Recall, F1** all near **1.0** (excellent performance)
