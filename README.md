# phishing-detection-4way
A BERT‐based 4-way phishing detector that classifies text/URLs as legit or phishing (email vs URL).
---

We fine-tuned a pre-trained bert-base-uncased model on the cybersectony/PhishingEmailDetectionv2.0 dataset (120 000 training examples, 20 000 validation, 60 000 held-out test) to build a four-way phishing detector. The classifier learns to distinguish between legitimate emails, phishing emails, legitimate URLs, and phishing URLs. After tokenizing each sample to 64 tokens, we trained for three epochs at a learning rate of 2 × 10⁻⁵ with mixed-precision on a single GPU. On the test split, our model achieves approximately 92 % macro-averaged F1, demonstrating balanced performance across all four categories and strong generalization to unseen phishing and benign content.

---

predict one of four labels:

1. **Legit Email**   
2. **Phishing Email**   
3. **Legit URL**   
4. **Phishing URL**

5. ---

6. Dataset
7. We use the public cybersectony/PhishingEmailDetectionv2.0 dataset. 
