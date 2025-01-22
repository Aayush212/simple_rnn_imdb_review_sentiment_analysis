# simple_rnn_imdb_review_sentiment_analysis

# IMDB Movie Review Sentiment Analysis

This project implements a sentiment analysis model that classifies IMDB movie reviews as either **positive** or **negative** using a pre-trained **Simple RNN** model. The app is built using **Streamlit** for the user interface and **TensorFlow/Keras** for the model.

## Features

- **Text Preprocessing**: The model preprocesses the user input by tokenizing and padding the text to match the model's expected input format.
- **Prediction**: The app predicts whether the review sentiment is positive or negative.
- **Streamlit Interface**: The user can input a movie review, and the app will display the predicted sentiment along with a prediction score.

## Prerequisites

To run this project locally, ensure you have the following installed:

- Python 3.7+
- TensorFlow 2.x
- Streamlit
- Other dependencies listed in `requirements.txt`

## Setup Instructions

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Aayush212/simple_rnn_imdb_review_sentiment_analysis.git
   cd imdb-sentiment-analysis
   ```

2. **Create a Virtual Environment** (optional but recommended):

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment**:
   - **Windows**:
     ```bash
     venv\Scripts\activate
     ```
   - **Mac/Linux**:
     ```bash
     source venv/bin/activate
     ```

4. **Install the Dependencies**:

   Install the required libraries using `pip`:

   ```bash
   pip install -r requirements.txt
   ```

   If you don't have `requirements.txt`, you can install the dependencies manually:

   ```bash
   pip install tensorflow streamlit numpy
   ```

5. **Download the Pre-trained Model**:
   Ensure that the pre-trained model (`simple_rnn_imdb.h5`) is in the same directory as the `main.py` file.

6. **Run the Streamlit App**:

   Start the app with the following command:

   ```bash
   python -m streamlit run main.py
   ```

   You can now view the app in your browser at [https://simplernnimdbreviewsentimentanalysis-ycqkri2h2ftp6rdrg2cqdd.streamlit.app/].

## How It Works

1. **Text Preprocessing**: The app takes the movie review input from the user, converts it into a sequence of integers (using the IMDB word index), and pads it to ensure consistent input size.

2. **Prediction**: The preprocessed review is passed through the pre-trained Simple RNN model, which outputs a sentiment score. The app classifies the sentiment as either **positive** or **negative** based on this score.

3. **Results**: The sentiment and prediction score are displayed on the Streamlit interface.

## Code Structure

- `main.py`: Main script for running the Streamlit app and performing sentiment analysis.
- `simple_rnn_imdb.h5`: Pre-trained Simple RNN model file (ensure it is in the same directory).
- `requirements.txt`: List of dependencies for the project.

## Requirements

- Python 3.7+
- TensorFlow 2.x
- Streamlit
- numpy

## Contributing

Feel free to fork this repository, make changes, and submit a pull request. If you have any suggestions or improvements, please open an issue or contribute directly!

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

