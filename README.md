# SoloHex-26
Nowadays, a lot of fake news is spreading on social media, which creates  confusion among people. An AI-based system can be developed to identify  whether the news is real or fake. 
Features:
[1]Detects the fake news using rule-based logic(Keywords).
[2]Simple web interface built with HTML, CSS, and Flask(Framework).
[3]User-friendly input form with validation for accurate results.
[4]Instant feedback on the authenticity of news articles.

Technologies:
[1]Python
[2]Flask (Web framework, for backend logic handling)
[3]HTML & CSS
[4]Rule-based validation logic

Working &  Logic:
1. User inputs news text.
2. Text is preprocessed (cleaning, tokenization, stopwords removal).
3. ML model predicts whether news is real or fake.
4. Result displayed on web interface.

#Code[ Full Availabe in app.py]
# Function to Predict whether: Fake
fake_keywords = ["clickbait", "shocking", "unbelievable", "hoax", "Rumor"]
def predict_news_rule_based(text):
    for word in fake_keywords:
        if word.lower() in text.lower():
            return "Fake"
    return "Real"
