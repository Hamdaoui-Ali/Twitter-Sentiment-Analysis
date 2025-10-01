# 🐦 Twitter Sentiment Analysis

A powerful real-time sentiment analysis application that analyzes text sentiment and Twitter data using machine learning. Built with Streamlit, scikit-learn, and NLTK.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3+-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## ✨ Features

- **Real-time Text Analysis**: Analyze sentiment of any text input instantly
- **Twitter Integration**: Fetch and analyze tweets from any Twitter user
- **Machine Learning Model**: Trained on 1.6M tweets with 80% accuracy
- **Beautiful UI**: Clean, responsive interface with color-coded results
- **Preprocessing Pipeline**: Advanced text cleaning, stopword removal, and TF-IDF vectorization
- **Error Handling**: Robust error handling for Twitter API limitations

## 🚀 Live Demo

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://your-app-url.streamlit.app)

## 📊 Model Performance

- **Dataset**: 1.6 million processed tweets
- **Accuracy**: 79.9%
- **Algorithm**: Logistic Regression with TF-IDF vectorization
- **Features**: 16,092 unique features from text preprocessing

## 🛠️ Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/twitter-sentiment-analysis.git
   cd twitter-sentiment-analysis
   ```

2. **Create virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**

   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   Navigate to `http://localhost:8501`

## 📁 Project Structure

```
twitter_sentiment_analysis/
├── app.py                              # Main Streamlit application
├── model_corrected.pkl                 # Trained machine learning model
├── vectorizer_corrected.pkl            # TF-IDF vectorizer
├── twitter_sentiment_analysis.ipynb    # Jupyter notebook for training
├── training.1600000.processed.noemoticon.csv  # Training dataset
├── requirements.txt                    # Python dependencies
└── README.md                          # Project documentation
```

## 🎯 Usage

### Text Analysis

1. Select "Input text" option
2. Enter your text in the text area
3. Click "Analyze" to get sentiment prediction
4. View results with color-coded indicators

### Twitter Analysis

1. Select "Get tweets from user" option
2. Enter a Twitter username
3. Click "Fetch Tweets" to analyze recent tweets
4. View sentiment analysis for each tweet

## 🔧 Technical Details

### Machine Learning Pipeline

- **Text Preprocessing**:
  - Remove non-alphabetic characters
  - Convert to lowercase
  - Remove stopwords
  - Tokenization
- **Feature Extraction**: TF-IDF vectorization
- **Model**: Logistic Regression classifier
- **Evaluation**: 80/20 train-test split

### Technologies Used

- **Frontend**: Streamlit
- **ML Framework**: scikit-learn
- **NLP**: NLTK
- **Data Processing**: pandas, numpy
- **Twitter Scraping**: ntscraper

## 📈 Dataset Information

The model is trained on the Sentiment140 dataset:

- **Size**: 1.6 million tweets
- **Labels**: Positive (4) and Negative (0)
- **Format**: CSV with columns: target, id, date, flag, user, text
- **Preprocessing**: Cleaned and processed for optimal performance

## 🚨 Important Notes

- **Twitter API**: The Twitter scraping feature may have limitations due to API restrictions
- **Model Files**: The corrected model files (`model_corrected.pkl`, `vectorizer_corrected.pkl`) are included
- **Dependencies**: All required packages are listed in `requirements.txt`

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Sentiment140 dataset creators
- Streamlit team for the amazing framework
- scikit-learn community
- NLTK contributors


---

⭐ **Star this repository if you found it helpful!**
