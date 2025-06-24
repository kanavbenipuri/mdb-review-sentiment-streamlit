# IMDB Sentiment Analysis Streamlit App

This project provides a web application for sentiment analysis of IMDB movie reviews using a pre-trained Simple RNN model in TensorFlow/Keras. The app is built with Streamlit for easy user interaction.

## Features
- Classifies user-input movie reviews as Positive or Negative
- Uses a pre-trained model (`simple_rnn_imdb.h5`) trained on the IMDB dataset
- Handles out-of-vocabulary words robustly
- Simple, interactive web interface

## Files
- `main.py`: Streamlit app for sentiment analysis
- `simple_rnn_imdb.h5`: Pre-trained Keras model
- `requirements.txt`: Python dependencies
- `prediction.ipynb`: Jupyter notebook for model prediction and testing

## Getting Started

### 1. Clone the repository
```
git clone https://github.com/yourusername/imdb-sentiment-streamlit.git
cd imdb-sentiment-streamlit
```

### 2. Set up a virtual environment (optional but recommended)
```
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate
```

### 3. Install dependencies
```
pip install -r requirements.txt
```

### 4. Run the Streamlit app
```
streamlit run main.py
```

## Usage
- Enter a movie review in the text area.
- Click the "Classify" button to see the sentiment prediction and score.

## Notes
- The model expects reviews in English.
- Only the top 10,000 words from the IMDB dataset are recognized; others are treated as unknown.

## License
This project is for educational purposes.
