# Fine-Grained Sentiment Analysis of Yelp Reviews Using BERT

This repository contains the code for fine-grained multi-class sentiment classification of Yelp reviews using a BERT-based model. The task is to predict star ratings (1 to 5) based on review text.

## Project Highlights

- Uses the Yelp Review Full dataset (subset for faster training)
- Preprocessing includes text cleaning and tokenization with Hugging Face's `AutoTokenizer`
- Fine-tunes `bert-base-uncased` model with customized dropout rates to reduce overfitting
- Implements training with early stopping and mixed precision (fp16)
- Evaluates using accuracy and macro F1-score
- Includes scripts for data preprocessing, model training, evaluation, and inference on sample texts

📊 Results

- Accuracy: ~63.5%
- Macro F1-score: ~0.64
- Model performs best on extreme ratings (1 and 5 stars)

📌 Notes

- Used a subset of 10,000 training and 1,000 test samples due to resource limits
- Future improvements: better class balance, data augmentation, or larger model
