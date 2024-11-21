# Movie Review Sentiment Analysis

## Project Description
This project aims to develop a system for filtering and categorizing movie reviews to automatically detect negative sentiments using machine learning models.


## Project Structure
- `data/`: Contains dataset files.
- `scripts/`: Includes preprocessing, training, and evaluation scripts.
- `models/`: Saved model files.

## Models Used
- Logistic Regression
- Gradient Boosting
- [Any others]
- Exploration with BERT embeddings for a subset of data

## Evaluation Metrics
The models are evaluated primarily using the F1 score, aiming for a threshold of 0.85.

## Results and Conclusions
Conclusion After testing three different models on custom reviews, I've observed the following:

Model Performance: Model 1: Achieved moderate confidence levels on positive reviews but struggled with highly negative reviews, indicating potential overfitting to certain patterns. Model 2: Demonstrated the lowest probability scores for negative sentiments, suggesting it may be underperforming in capturing subtle negative cues. Model 3: Provided consistent and balanced scores across different reviews, indicating it could generalize better on varied inputs.

Preprocessing Effects: spaCy Preprocessing: Improved the models' ability to capture sentiment nuances by lemmatizing and reducing noise, especially for Model 3. TF-IDF Vectorization: Proved effective in distinguishing between positive and negative sentiment, though performance varied based on the initial preprocessing steps.

Recommendations: Further hyperparameter tuning may improve probabilities for edge cases. Incorporating additional sentiment-related features, such as negation handling, could enhance the models' accuracy.
