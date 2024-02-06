# What is Sentiment Analysis? 
- **Definition:** Sentiment Analysis, also known as Opinion Mining, is an Classification use-case that employes NLP techniques to classify a given text into various sentiments, such as positive or negative, Happy, Sad or Neutral, etc. In simple terms, it is the process of detecting positive or negative sentiment in a text. 


- **Objectives:** The key aim of Sentiment Analysis is to categorize opinions expressed in a piece of text, determining the writer's attitude towards a particular subject (topic, product, etc.). 


- **Applications:** Sentiment analysis helps with public opinion analysis on social media posts, customer reviews, or news articles. For example, analyzing Twitter data to determine the overall sentiment towards a particular product or tracking customer sentiment in online reviews. It is often used by businesses to detect sentiment in social data, gauge brand reputation, and understand customers.


# Types of Sentiment Analysis:

1. **Standard Sentiment Analysis:**
   - Classifies text into one of three sentiments: Positive, Negative, Neutral.
   - Example: "I love this product" → Positive, "I hate waiting" → Negative, "The weather is okay" → Neutral.
   - Different methods to implement Standard Sentiment Analysis are executed in this notebook. 

2. **Graded Sentiment Analysis:**
   - Also known as Fine-Grained Sentiment Analysis, Classifies text into one of five sentiments on a scale: Very Positive, Positive, Neutral, Negative, Very Negative.
   - Example: "The movie was amazing!" → Very Positive, "The service was okay" → Neutral, "I'm extremely disappointed" → Very Negative.
   - In implementation terms, it is an ML model trained on a labelled dataset that contains "Very Positive, Positive, Neutral, Negative, Very Negative" values in its target variable. 

3. **Intent Analysis:**
   - Determines the intent behind the text, identifying the user's purpose or goal.
   - Example: "I want to purchase a new laptop" → Intent: Purchase, "I need information about your services" → Intent: Inquiry.
   - In implementation terms, it is an ML model trained on a labelled dataset that contains the target variable "Intent" along with the target variable "Sentiment". It is a classical case of Multi-Label Text-Classification. 

4. **Emotion Detection Sentiment Analysis:**
   - Identifies specific emotions expressed in text: Happy, Sad, Fear, Anger, Disgust, Surprise, etc.
   - Example: "I'm thrilled to hear the news!" → Happy, "This story is heartbreaking" → Sad.
   - In implementation terms, it is an ML model trained on a labelled dataset that contains the target variable "Emotion". 

5. **Aspect-based Sentiment Analysis:**
   - Analyzes text to determine sentiments related to specific aspects or features mentioned.
   - Example: "The phone has a great camera, but the battery life is disappointing" → Positive aspect: Camera, Negative aspect: Battery Life.
   - In implementation terms, it is an ML model trained on a labelled dataset that contains the target variable "Aspect" along with the target variable "Sentiment". It is a classical case of Multi-Label Text-Classification. 

_Sentiment Analysis can be further extended into multiple use-cases, custom-tailored with features like Multilingual Support, Urgency Detection, and more._


# Methods to Implement Sentiment Analysis using Python

1. **Pre-Trained NLP Libraries:**
   - Certain Python libraries like NLTK, Textblob provide ready-to-use pretrained Sentiment Analysis models that need no further training.
   - These pre-trained models offer generic sentiment analysis and are not domain-specific.

2. **Rule-based Systems:**
   - Uses a set of human-crafted rules to help identify subjectivity, polarity, or the subject of an opinion.
   - In this approach, each word (or lexicon) in the dictionary is assigned a sentiment score (i.e., a number from -1.0 to +1.0).
   - _The rule-based processes are intensive, domain-specific, and need an SME to craft precise rules during creation and timely maintenance. Hence, not included in this notebook._

3. **Machine Learning Systems (ML):**
   - A sentiment analysis task is usually modeled as a classification problem, whereby a classifier model is fed a text and returns a category, e.g., positive, negative, or neutral.
   - This involves training the classifier model from scratch on custom-labeled training data, evaluation, fine-tuning, and real-time testing.

4. **Deep Learning Systems (DL):**
   - Similar to the Machine Learning approach, but instead of a statistic classifier model, a Deep Neural Network based model is employed.
   - This involves training the Neural Network classifier model from scratch or apply Transfer Learning on a pre-trained Deep Neural Network Model on custom-labeled training data.

5. **SaaS Products (Free/Purchase):**
   - Usually come as a SaaS bundle with attached Tableau/PowerBI dashboards for user-friendly visualizations.
   - These are no-code sentiment analysis solutions for large-scale data-visualization tasks that recur every day.

_"Sentiment analysis is one of the hardest tasks in natural language processing, because even humans struggle to analyze sentiments accurately."_


# References: 
- https://www.analyticsvidhya.com/blog/2022/07/sentiment-analysis-using-python/
- https://monkeylearn.com/sentiment-analysis/
- https://github.com/hansmichaels/sentiment-analysis-IMDB-Review-using-LSTM/tree/master
- https://colab.research.google.com/drive/1UmwEbi6O_2epPsTcDqYkJdoZdWIiaQux?usp=sharing
- EDA for Sentiment Analysis: https://www.kaggle.com/code/tanulsingh077/twitter-sentiment-extaction-analysis-eda-and-model/notebook