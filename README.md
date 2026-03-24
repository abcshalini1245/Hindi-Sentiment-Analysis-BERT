# 🇮🇳 Vernacular Hindi Sentiment Analysis (BERT)

A specialized NLP pipeline designed to analyze sentiment in Hindi video comments. This project focuses on overcoming "Majority Class Bias" using cost-sensitive learning.

## 🧠 Technical Highlights
- **Base Model:** `l3cube-pune/hindi-bert-v2` (Monolingual Hindi BERT).
- **Optimization:** Implemented a **Custom Weighted Cross-Entropy Loss** (Weights: Neg=2.0, Neu=1.5, Pos=1.0) to ensure the model doesn't ignore negative feedback.
- **Accuracy:** ~80% on 3-class classification (Positive, Negative, Neutral).

## 📁 Project Structure
- `Hindi_Sentiment_Analysis.ipynb`: Full training and evaluation pipeline.
- `analyzed_feedback.csv`: Example output of the batch-processing engine.
- `requirements.txt`: Environment dependencies.

## 📊 Performance (Confusion Matrix)
The model shows strong diagonal performance, successfully distinguishing between Neutral and Negative sentiments which are often confused in multilingual models.

## 🚀 Future Scope
Integrating this engine with **OpenAI Whisper ASR** to analyze the sentiment of spoken Hindi stories for platforms like Josh Talks.
