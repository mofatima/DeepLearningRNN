# Simplernn-sentiment-analysis

# IMDB Movie Review Sentiment Analysis using SimpleRNN

## Overview
In this project I have used a sentiment analysis model using a Simple Recurrent Neural Network (SimpleRNN). The model is trained on the IMDB dataset to classify movie reviews as either positive or negative. A Streamlit web app is provided for user interaction, allowing users to input a review and receive a sentiment prediction.

## Features
- Uses TensorFlow/Keras for model training and inference
- Pre-trained SimpleRNN model loaded from `simple_rnn_imdb.h5`
- IMDB dataset for training and testing
- Streamlit-based web interface for real-time sentiment classification

## Installation

### Install dependencies
```bash
pip install -r requirements.txt
```

### Install additional dependencies if needed
```bash
pip install tensorflow numpy streamlit
```

## Usage
1. Clone the repository:
```bash
git clone <repository-url>
cd simplernn_sentiment_analysis
```

2. Run the Streamlit app:
```bash
streamlit run main.py
```

3. Enter a movie review in the text area and click **Classify** to see the sentiment prediction.

## Dataset
- IMDB Movie Review dataset (preloaded from `tensorflow.keras.datasets.imdb`)
- Reviews are preprocessed using tokenization and padding (max length = 500 words)

## Model Details
- **Embedding Layer**: Converts words into dense vectors
- **SimpleRNN Layer**: Captures sequential dependencies in text
- **Dense Layer with ReLU Activation**: Processes RNN outputs
- **Output Layer with Sigmoid Activation**: Provides binary classification (positive/negative)
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam

## Results
- The model predicts sentiment with reasonable accuracy on unseen reviews.
- Streamlit UI allows easy interaction with the model.

## Future Improvements
- Train a more robust model using LSTMs/GRUs for better sequential understanding.
- Deploy the model on cloud services for broader accessibility.
- Improve UI/UX for better user experience.

## Contributing
Feel free to fork this project and contribute by submitting pull requests.


