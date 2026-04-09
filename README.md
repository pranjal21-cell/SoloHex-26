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

    #Installation:
    Flask==2.3.0
    pandas==2.0.3
    
#Flowchart:
<img width="571" height="362" alt="image" src="https://github.com/user-attachments/assets/f9a116bf-bb51-41d7-9275-c5ce45851cda" />

#Table Defining [Fake keywords, Real Keywords, Suspicious Keywords]:
 Rule No.  Keyword / Pattern       | Type       | Description / Reason for Flagging            

 1       | clickbait               | Suspicious | Exaggerated headline to attract clicks       
 2       | shocking / unbelievable | Suspicious | Sensational phrases to grab attention        
 3       | hoax                    | Fake/Rumor | Indicates deliberately false information     
 4       | rumor                   | Fake/Rumor | Suggests unverified or circulating claims    
 5       | viral                   | Suspicious | Often used to exaggerate or mislead          
 6       | conspiracy              | Fake/Rumor | Indicates content may be misleading or false 
 7       | unverified              | Fake/Rumor | Explicitly shows the news is not confirmed   
 8       | fake news               | Fake/Rumor | Keyword directly indicating false content    
 9       | unbelievable story      | Suspicious | Sensational story that may mislead           
 10      | alert / urgent          | Suspicious | Often used to provoke fear or clicks         

