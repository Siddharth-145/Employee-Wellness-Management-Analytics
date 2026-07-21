# Employee Wellness Management Analytics

## Milestone 2 – NLP Text Preprocessing Pipeline

---

## Project Objective

The objective of this milestone is to develop a multilingual NLP preprocessing pipeline capable of preparing raw employee feedback for sentiment and emotion analysis. The pipeline accepts text from user input or uploaded files, performs language detection, applies various preprocessing techniques, and displays intermediate outputs generated during each preprocessing stage.

---

## NLP Pipeline Overview

The implemented pipeline performs the following tasks:

- Text Input (TXT / CSV)
- Language Detection
- Unicode Normalization
- Text Cleaning
- URL Removal
- Email Removal
- HTML Tag Removal
- Emoji Extraction
- Punctuation Removal
- Number Removal
- Lowercase Conversion
- Tokenization
- Stop-word Removal
- Lemmatization
- Noise Filtering
- Final Preprocessed Text Generation

---

## Technologies and Libraries Used

- Python
- Google Colab
- Streamlit
- FastAPI
- Pandas
- NLTK
- spaCy
- langdetect
- emoji
- regex
- HTML Parser (BeautifulSoup)

---

## Google Colab Setup Instructions

1. Open the notebook in Google Colab.
2. Install the required libraries.
3. Run all notebook cells sequentially.
4. Upload a TXT or CSV file.
5. Execute the preprocessing pipeline.
6. Observe intermediate preprocessing outputs.

---

## Preprocessing Workflow

Input Text

↓

Language Detection

↓

Unicode Normalization

↓

Text Cleaning

↓

Emoji Extraction

↓

URL / Email / HTML Removal

↓

Punctuation & Number Removal

↓

Tokenization

↓

Stop-word Removal

↓

Lemmatization

↓

Noise Filtering

↓

Final Preprocessed Text

↓

Sentiment & Emotion Ready Output

---

## Sample Input

```
I am very happy 😊 with the workplace.
```

---

## Sample Output

Language Detected:

```
English
```

Extracted Emoji

```
😊
```

Final Preprocessed Text

```
happy workplace
```

---

## Observations

- Successfully supports multilingual text.
- Displays intermediate outputs after every preprocessing stage.
- Handles unsupported languages gracefully.
- Generates clean text suitable for sentiment and emotion analysis.
- Provides an intuitive interface using Streamlit.