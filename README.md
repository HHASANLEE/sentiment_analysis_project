# Sentiment Analysis Project
Problem Description
Users share thousands of opinions daily on online platforms about various products, services, and topics. These text data are valuable sources of information for businesses and analysts. However, manual analysis of such a large volume of data is not feasible. Therefore, there is a need for AI-based approaches that can automatically determine the emotional tone (positive, negative, or neutral) of texts.

## Approach
In this project, we employed both:

A rule-based method (VADER – Valence Aware Dictionary for Sentiment Reasoning), and

A deep learning-based method (RoBERTa – a transformer-based pre-trained model).

We analyzed the sentiment of sentences using both models and compared the results.

## Proposed Solution
The project developed a system that automatically identifies the sentiment of user sentences.
The system provides results from two models:

VADER: Returns compound, positive, neutral, and negative scores.

RoBERTa: Returns roberta_pos, roberta_neu, and roberta_neg scores.

Additionally, the system supports real-time testing:
Users can input any sentence and instantly receive its sentiment analysis.

## How It Was Implemented
Dataset: The SENTIMENT101 twitter comments dataset was loaded from the Kaggle platform.

Processing: Each sentence was analyzed first using the VADER model and then with the RoBERTa model.

Merging: Results from both models were combined into a single DataFrame.

Visualization: Sentiment scores were visualized using Seaborn and Matplotlib libraries.

Real-Time Testing: A function was created to allow users to input any custom sentence and get an immediate sentiment result.


