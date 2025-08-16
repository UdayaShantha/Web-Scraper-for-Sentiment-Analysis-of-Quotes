# Web-Scraper-for-Sentiment-Analysis-of-Quotes
The project aims to develop a system that automatically extracts quotes from a website, preprocesses the text, and performs sentiment analysis to classify the sentiment of each quote.Sentiment analysis is a critical task in understanding public opinion, brand monitoring, and gaining insights from textual data. This project showcases the integration of web scraping, natural language processing (NLP), and machine learning techniques.


## Machine Learning Approach and Justification

The project applies a Support Vector Machine (SVM) classifier to perform sentiment analysis on the scraped quotes.
Why SVM?
• SVM is effective in high-dimensional spaces, making it suitable for text classification tasks.
• SVM can handle non-linear data through the use of different kernel functions.
Machine Learning Pipeline:
1. Text Preprocessing:
• Tokenization: The raw text is broken down into individual words or tokens using word_tokenize.
• Stop Word Removal: Common English words (e.g., "the," "and") are removed using stopwords.words('english').
• Lemmatization: Words are reduced to their base or dictionary form using WordNetLemmatizer.
2. Feature Extraction:
• TF-IDF Vectorization: The preprocessed text is converted into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency). TF-IDF measures the importance of each word in the document relative to the entire corpus.
3. Model Training:
• The SVM model is trained on the TF-IDF vectors using the training dataset.
4. Model Evaluation:
• The trained model is evaluated on the testing dataset using metrics such as precision, recall, F1-score, and confusion matrix.
