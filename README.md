📝 Text Preprocessing using NLTK & SpaCy
Natural Language Processing (NLP) begins with text preprocessing. This project demonstrates essential text preprocessing techniques such as tokenization, stemming, lemmatization, and stopword removal using Python libraries like NLTK and SpaCy.
🚀 Open in Google Colab


📌 Overview
Text preprocessing is a crucial step in NLP pipelines. Raw text data often contains punctuation, stopwords, and inconsistent formatting that can negatively affect machine learning models.
This notebook demonstrates various preprocessing techniques used to clean and prepare textual data for NLP applications.

✨ Features
✅ Word Tokenization
✅ Sentence Tokenization
✅ Character Tokenization
✅ Stemming using Porter Stemmer
✅ Lemmatization using WordNet Lemmatizer
✅ Stopword Removal using NLTK
✅ Stopword Removal using SpaCy
✅ End-to-End Text Preprocessing Pipeline

🛠 Technologies Used


Python


NLTK


SpaCy


Google Colab


Jupyter Notebook



📚 Concepts Covered
1️⃣ Word Tokenization
Breaks a sentence into individual words.
Example
from nltk.tokenize import word_tokenizetext = "I love learning NLP."tokens = word_tokenize(text)print(tokens)
Output
['I', 'love', 'learning', 'NLP', '.']

2️⃣ Sentence Tokenization
Splits text into individual sentences.
from nltk.tokenize import sent_tokenizetext = "I love AI. NLP is amazing."sentences = sent_tokenize(text)print(sentences)

3️⃣ Character Tokenization
Converts text into individual characters.
text = "Hello"tokens = list(text)print(tokens)
Output
['H', 'e', 'l', 'l', 'o']

4️⃣ Stemming
Reduces words to their root form by removing suffixes.
from nltk.stem import PorterStemmerstemmer = PorterStemmer()words = ["running", "playing", "studies"]for word in words:    print(stemmer.stem(word))

5️⃣ Lemmatization
Converts words to their meaningful base dictionary form.
from nltk.stem import WordNetLemmatizerlemmatizer = WordNetLemmatizer()words = ["running", "studies", "cars"]for word in words:    print(lemmatizer.lemmatize(word))

6️⃣ Stopword Removal using NLTK
Removes common words that add little meaning.
from nltk.corpus import stopwordsfrom nltk.tokenize import word_tokenize
Example:
Original:The cat is sitting on the mat.After Removal:cat sitting mat

7️⃣ Stopword Removal using SpaCy
Uses SpaCy's built-in stopword list for text cleaning.
import spacynlp = spacy.load("en_core_web_sm")

8️⃣ Complete NLP Preprocessing Pipeline
The notebook combines:


Tokenization


Stemming


Lemmatization


Stopword Removal


to create a complete preprocessing workflow.

📂 Project Structure
Text_Preprocessing.ipynbREADME.md

🎯 Learning Outcomes
By completing this notebook, you will learn:


Fundamentals of NLP preprocessing


How tokenization works


Difference between stemming and lemmatization


How to remove stopwords effectively


Building preprocessing pipelines for NLP tasks



🌟 Real-World Applications
Chatbots
Clean user messages before processing.
Sentiment Analysis
Prepare customer reviews for classification.
Spam Detection
Extract meaningful words from emails.
Search Engines
Improve keyword matching and relevance.
Text Classification
Enhance model accuracy with cleaned text.

📊 Libraries Installation
pip install nltkpip install spacy
Download required NLTK resources:
import nltknltk.download('punkt')nltk.download('wordnet')nltk.download('stopwords')
Download SpaCy model:
python -m spacy download en_core_web_sm

▶️ How to Run
Clone Repository
git clone https://github.com/your-username/text-preprocessing-nlp.git
Install Dependencies
pip install nltk spacy
Open Notebook
jupyter notebook Text_preprocessing.ipynb
Or run directly in Google Colab using the badge above.

🔮 Future Enhancements


TF-IDF Vectorization


Bag of Words (BoW)


Word Embeddings


Named Entity Recognition (NER)


POS Tagging


Text Classification Models


Sentiment Analysis Projects



👨‍💻 Author
Gnani Tadiparthi
Aspiring AI Engineer passionate about Machine Learning, Natural Language Processing, Generative AI, and Data Science.
Connect with Me


GitHub: https://github.com/gnani291



⭐ Support
If you found this project helpful:
⭐ Star the repository
🍴 Fork the project
📢 Share it with others interested in NLP
