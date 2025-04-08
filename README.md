
# 🧠 Web Article - Text Mining

## 📝 Objective

This project focuses on **text extraction and natural language processing** to analyze articles from a list of URLs provided in `Input.xlsx`. The goal is to extract the article content and compute a set of textual and linguistic metrics as outlined in the assignment instructions.

---

## 📂 Project Structure

```
NLP-Assignment/
│
├── code.py                     # Python script for scraping and text analysis
├── Input.xlsx                  # Contains URLs and URL_IDs
├── Output Data Structure.xlsx # Defines the format and variables for the final output
├── Output.csv                  # Final output file with calculated text features
├── extracted_articles/        # Folder containing .txt files for each extracted article
├── stopwords/                 # Folder containing stopwords files used in analysis
│   ├── stopwords-*.txt
├── master_dictionary/         # Folder containing positive and negative word dictionaries
│   ├── positive-words.txt
│   ├── negative-words.txt
└── README.md                  # You’re reading it now!
```

---

## ⚙️ Technologies Used

- Python
- `requests`, `BeautifulSoup` – for web scraping
- `nltk`, `re`, `textstat` – for NLP and text feature analysis
- `openpyxl`, `pandas` – for reading and writing Excel files

---

## 🧪 Text Analysis Metrics Computed

Following variables are calculated for each article:

- ✅ POSITIVE SCORE  
- ❌ NEGATIVE SCORE  
- ⚖️ POLARITY SCORE  
- 🧠 SUBJECTIVITY SCORE  
- 📏 AVG SENTENCE LENGTH  
- 📊 PERCENTAGE OF COMPLEX WORDS  
- 🌫️ FOG INDEX  
- 🔤 AVG NUMBER OF WORDS PER SENTENCE  
- 🧩 COMPLEX WORD COUNT  
- 🔢 WORD COUNT  
- 🔠 SYLLABLE PER WORD  
- 👤 PERSONAL PRONOUNS  
- 📉 AVG WORD LENGTH  

These metrics help in understanding the sentiment, readability, and linguistic structure of the articles.

---

## 🚀 How to Run

### ✅ Prerequisites

Install required dependencies:

```
pip install -r requirements.txt
```

> Example `requirements.txt` content:
```
beautifulsoup4
requests
pandas
openpyxl
nltk
textstat
```

### 🧾 Steps to Execute

1. **Place the `Input.xlsx`** and **required folders** (`stopwords`, `master_dictionary`) in the same directory as your script.
2. Run the script:

```
python code.py
```

3. The script will:
   - Scrape each article and save it to `extracted_articles/` as a `.txt` file
   - Analyze each text and compute the required metrics
   - Save the results into `Output.csv`
