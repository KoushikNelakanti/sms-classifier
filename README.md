# 📱 SMS Spam Classifier

A machine learning web application that classifies SMS messages as **Spam** or **Ham** using Naive Bayes and TF-IDF vectorization.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Accuracy](https://img.shields.io/badge/Accuracy-97%25-brightgreen.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-Enabled-red.svg)

---

## 🚀 Features

- **Interactive Web Interface**: Beautiful Streamlit UI for easy message classification
- **Real-time Results**: Instant spam detection with visual feedback
- **Confidence Scoring**: See how certain the model is about each prediction
- **User-friendly Design**: Clean, intuitive interface anyone can use

---

## 📁 Project Structure

```
sms-spam-classifier/
├── main.py              # Model training script
├── spam_app.py          # Streamlit web application
├── predict.py           # Command-line prediction tool
├── utils.py             # Text preprocessing utilities
├── model.pkl            # Trained Naive Bayes model
├── vectorizer.pkl       # TF-IDF vectorizer
├── requirements.txt     # Python dependencies
└── README.md           # Project documentation
```

---

## ⚡ Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/koushikbinary01/sms-spam-classifier.git
cd sms-spam-classifier
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Train Model (Optional)
```bash
python main.py
```

### 4. 🌐 Launch Web App
```bash
streamlit run spam_app.py
```
*The app will open automatically in your browser at `http://localhost:8501`*

### 5. 💻 Command Line Tool (Optional)
```bash
python predict.py
```

---

## 🎯 Usage

### 🌐 Web Interface (Recommended)
1. Launch the Streamlit app: `streamlit run spam_app.py`
2. Open your browser to `http://localhost:8501`
3. Enter any SMS message in the text area
4. Click **"Classify Message"** 
5. Get instant results with confidence score!

**Example:**
- Input: `"FREE! Claim your prize now! Click here!!!"`
- Output: `🚨 SPAM (Confidence: 98.7%)`

### 💻 Command Line (Alternative)
```bash
python predict.py
# Follow the prompts to enter your message
```

---

## 📊 Model Performance

- **Accuracy**: ~97%
- **Algorithm**: Multinomial Naive Bayes
- **Vectorization**: TF-IDF (Term Frequency-Inverse Document Frequency)
- **Text Processing**: NLTK preprocessing pipeline

---

## 🛠️ Technical Details

### Dependencies
- **streamlit**: Web application framework
- **scikit-learn**: Machine learning library
- **nltk**: Natural language processing
- **pandas**: Data manipulation
- **numpy**: Numerical computing
- **joblib**: Model serialization

### Model Pipeline
1. Text preprocessing (cleaning, tokenization)
2. TF-IDF feature extraction
3. Naive Bayes classification
4. Prediction with confidence score

---

## 🔧 File Descriptions

| File | Purpose |
|------|---------|
| `main.py` | Trains the spam classifier model |
| `spam_app.py` | Streamlit web interface |
| `predict.py` | CLI tool for predictions |
| `utils.py` | Text preprocessing functions |
| `model.pkl` | Serialized trained model |
| `vectorizer.pkl` | Serialized TF-IDF vectorizer |
| `requirements.txt` | Python package dependencies |

---

## 📋 Requirements

```txt
streamlit>=1.28.0
scikit-learn>=1.3.0
nltk>=3.8
pandas>=2.0.0
numpy>=1.24.0
joblib>=1.3.0
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## 📄 License

MIT License - feel free to use this project for learning and development.

---

## 👨‍💻 Author

**Koushik Nelakanti**  
GitHub: [@KoushikNelakanti](https://github.com/KoushikNelakanti)

---

⭐ **If you found this project helpful, please give it a star!**