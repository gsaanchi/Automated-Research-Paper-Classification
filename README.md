# NLP-Based Research Paper Classification

This repository contains an end-to-end Machine Learning pipeline to automate the process of categorizing research papers on academic submission platforms. By analyzing the title and abstract of submitted papers, this system predicts the most relevant categories across 57 distinct classes, streamlining the submission workflow and enhancing user experience.

---

## 📌 Project Overview

When submitting research papers, authors are traditionally required to manually select subject categories. Given the vast array of available domains, this task can be time-consuming and subjective. 

This solution leverages state-of-the-art Natural Language Processing (NLP) transformer models to automate the categorization process, suggesting relevant subject tags based on textual analysis of the paper's title and abstract.

---

## 🛠️ Models & Architecture

Several advanced transformer-based language models were fine-tuned for this multi-label classification task:

*   **RoBERTa**: A robustly optimized BERT approach utilizing dynamic masking and larger batch sizes for robust representation learning.
*   **DeBERTa**: Enhances RoBERTa with a disentangled attention mechanism and an enhanced mask decoder.
*   **DeBERTa-Large**: A larger scaling of DeBERTa providing stronger contextual embeddings.

An ensemble approach was implemented to combine prediction probabilities from each model, resulting in more stable and robust predictions.

### Performance
The combined ensemble model achieved a **Weighted F1 Score of 0.70**, demonstrating reliable performance across the 57 different target classes.

---

## 📂 Project Structure

This repository includes the following Jupyter notebooks:

*   **[DeBERTa Script](https://github.com/gsaanchi/Automated-Research-Paper-Classification/blob/main/deberta.ipynb)**: Code for training the base DeBERTa model.
*   **[DeBERTa Training Script (Alternative Configuration)](https://github.com/gsaanchi/Automated-Research-Paper-Classification/blob/main/deberta6.ipynb)**: Experimental DeBERTa training run.
*   **[DeBERTa-Large Script](https://github.com/gsaanchi/Automated-Research-Paper-Classification/blob/main/debertalarge.ipynb)**: Fine-tuning pipeline for the DeBERTa-Large model.
*   **[RoBERTa Script](https://github.com/gsaanchi/Automated-Research-Paper-Classification/blob/main/roberta3.ipynb)**: Training notebook for the RoBERTa model.
*   **[Inference Pipeline](https://github.com/gsaanchi/Automated-Research-Paper-Classification/blob/main/inference.ipynb)**: Complete end-to-end script for running inference and generating final predictions on unseen abstracts.

---

## 🚀 Future Scope

*   **Web Application**: Developing a Flask or FastAPI web interface to allow users to paste a title and abstract to receive real-time category predictions.
*   **Model Optimization**: Exploring lighter models (like DistilBERT) to reduce inference latency and computational overhead.

---

## 🤝 Contact & Contributions

Contributions and suggestions are welcome. Feel free to open an issue or submit a pull request.

**Author:** Saanchi Gupta 
**Email:** saanchigupta722004@gmail.com 
**GitHub:** [gsaanchi](https://github.com/gsaanchi)