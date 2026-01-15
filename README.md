# Multilingual BERT Sentiment Analysis
This project implements a multilingual sentiment analysis system using a BERT-based model. It classifies user comments as positive or negative by automatically detecting the input language and translating non-English text to English before sentiment prediction.
Run this notebook in Google Colab:https://colab.research.google.com/github/Anjali-sct27/Multilingual-BERT-Sentiment-Analysis/blob/main/Multilingual_BERT_Sentiment_Analysis_clean_ipynb.ipynb

## Project Description
User-generated content on social media and review platforms often appears in multiple languages. Traditional sentiment analysis systems usually work only for English text. This project addresses that limitation by combining language detection, machine translation, and a transformer-based sentiment classifier.
The system supports multiple Indian and global languages without requiring separate datasets for each language.

## Features
* Accepts text input in multiple languages
* Automatically detects the input language
* Translates non-English text to English
* Uses a BERT-based model for sentiment classification
* Classifies text into positive or negative sentiment

## Technologies Used
* Python
* HuggingFace Transformers
* DistilBERT (fine-tuned for sentiment analysis)
* MarianMT for translation
* langdetect
* Google Colab

## Workflow
1. User provides text input
2. Language of the input is detected
3. Text is translated to English if required
4. Sentiment is predicted using a BERT model

## Sample Outputs

### English Input
Input:I really love this app, it saves so much time
Output:Positive

### Tamil Input
Input:இந்த செயலி அருமையாக உள்ளது
Detected language: Tamil
Translated text: This app is very good
Output:Positive

### Hindi Input
Input:यह अनुभव बिल्कुल बेकार था
Detected language: Hindi
Translated text: This experience was absolutely useless
Output:Negative

### Korean Input
Input:이 앱은 정말 좋아요
Detected language: Korean
Translated text: This app is really good
Output:Positive

## How to Run
1. Open the notebook in Google Colab
2. Run all cells in order
3. Enter text in any supported language
4. View the predicted sentiment

## Limitations
* The model performs binary sentiment classification only
* Neutral sentences may be classified as positive
* Translation quality may vary slightly for some languages

## Future Improvements
* Add neutral sentiment classification
* Include confidence scores for predictions
* Improve translation accuracy using language-specific models
* Deploy the system as a web application

## Author
Anjali S Nair
B.Tech student with interest in AI, Machine Learning, and Natural Language Processing

Just tell me 👍
