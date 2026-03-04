# Comparative-ML-Models.ipynb
Comparative analysis of Neural Networks, Naive Bayes, and Random Forest classifiers on real-world dataset.

🎵 Lyrics-Based Genre Classification Using Machine Learning

📌 **Overview**
This project explores whether musical genre can be accurately classified using lyrics alone, without relying on audio-based features such as tempo, loudness, or spectral analysis.
Using the “Multilingual Lyrics for Genre Classification” dataset (≈250,000 songs across 10 genres), we implemented and compared three supervised machine learning models:

- Naive Bayes
- Neural Network
- Random Forest

The goal was to evaluate how effectively semantic patterns in song lyrics can predict genre classification.

🏛 **Symposium Presentation**

This research was presented at the Luddy Poster Symposium, where we demonstrated our comparative analysis of text-based genre classification models. The project included a formal research poster presentation outlining methodology, evaluation metrics, and model performance comparisons. I attached the poster in this repo.

📊 **Dataset**
Source: Kaggle – Multilingual Lyrics for Genre Classification
~250,000 songs
10 genres
Filtered to English-language songs for consistency

🧹 **Data Preprocessing**
Filtered for English-language entries
Removed punctuation, stop words, and line breaks
Converted all text to lowercase
Tokenized lyrics for feature extraction

🔎 **Feature Engineering**
We used TF-IDF vectorization with a maximum of 4,000 features to transform textual data into numerical vectors.
TF-IDF was selected to:
Emphasize genre-distinctive words
Reduce influence of high-frequency common words
Maintain computational efficiency at scale

🤖 **Models Implemented**

1️⃣ Naive Bayes (Baseline)
Fast training and inference
Assumes feature independence
Served as baseline for performance comparison

2️⃣ Neural Network
Captures nonlinear relationships in textual patterns
Improved performance over baseline
Demonstrated ability to model complex lyrical structure

3️⃣ Random Forest
Ensemble-based decision tree model
Achieved the strongest overall classification performance
Provided balanced precision and recall across genres

📈 **Evaluation Metrics**
Models were evaluated using:
Accuracy
Precision
Recall
F1 Score
Confusion Matrices (per genre breakdown)

🏆 **Results & Insights**
Naive Bayes was computationally efficient but limited by independence assumptions.
Neural Network significantly outperformed the baseline, indicating that lyrical context contains nonlinear patterns.

Random Forest achieved the best overall performance, suggesting ensemble methods are highly effective for text-based genre classification.
These findings demonstrate that lyrical semantics alone provide meaningful predictive signal for genre classification.

🔬 **Key Takeaways**
Lyrics contain measurable semantic patterns that correlate strongly with genre.
Ensemble models outperform linear probabilistic approaches in high-dimensional text spaces.
Model performance could likely improve further by integrating audio-based features.

🚀 **Future Work**
Integrate audio feature datasets (tempo, loudness, spectral features).
Explore deep learning NLP models (e.g., LSTM, transformers).
Experiment with word embeddings (Word2Vec, GloVe) instead of TF-IDF.

🛠 **Technologies Used**
Python
Pandas
NumPy
Scikit-learn
TensorFlow
Matplotlib
Seaborn

▶️ **How to Run**
1. Install dependencies:
pip install pandas numpy scikit-learn seaborn matplotlib tensorflow

2. Download dataset from Kaggle
https://www.kaggle.com/datasets/mateibejan/multilingual-lyrics-for-genre-classification

3. Place CSV files in the same directory as the notebook.
4. Run the notebook sequentially.
