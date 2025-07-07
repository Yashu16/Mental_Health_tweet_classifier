# 🧠 Mental Health Tweet Classifier

This project uses a BERT-based transformer model to classify tweets into two categories:
- **Mental Health**
- **Not Mental Health**

It leverages the power of **transformers** from Hugging Face to improve classification performance on short, noisy, and often emotionally charged Twitter data.

---

## 📌 Project Overview

- 🔍 **Problem:** Detect mental health-related tweets from general Twitter posts.
- 📊 **Dataset:** [Mental Health Twitter Dataset](https://www.kaggle.com/datasets/infamouscoder/mental-health-social-media) (10k+ tweets with labels)
- 🤖 **Model Used:** `bert-base-uncased` via Hugging Face Transformers
- 📈 **Final Evaluation:**
  - Accuracy: **94%**
  - F1 Score: **0.94**
  - Precision/Recall Balanced

---

## 📂 Project Structure

mental-health-tweet-classifier/
├── mental_health_classifier.ipynb # Full notebook with training pipeline
├── Mental-Health-Twitter.csv # Dataset
├── requirements.txt # Python dependencies
└── README.md # Project documentation

🧪 Model Training Summary
The model was trained for 3 epochs with TrainingArguments configured for evaluation on each epoch. Metrics were computed using sklearn.

Example output:

eval_accuracy: 0.94
eval_f1: 0.94
eval_precision: 0.95 (class 0), 0.94 (class 1)
eval_recall:    0.94 (class 0), 0.95 (class 1)

There are some mislabeled tweets in the dataset(eg. "Thank you so much" masked as mental health tweet)

🙌 Acknowledgements
Hugging Face 🤗 Transformers

scikit-learn

Dataset from Kaggle

📬 Contact
Built by Yaswanth kottana
Feel free to reach out if you'd like to collaborate or discuss ideas!

`In future I will be adding a web app to this project using streamlit`