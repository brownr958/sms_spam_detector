# SMS Spam Detector

This project is a simple machine learning application that classifies SMS text messages as spam or not spam using a Linear Support Vector Classifier (LinearSVC) and TF-IDF vectorization. The model is deployed with a Gradio interface, allowing users to interactively test messages.

## Files Included

- `gradio_sms_text_classification.ipynb`: The main Jupyter notebook containing model training, prediction logic, and the Gradio app interface.
- `sms_text_classification_solution.ipynb`: Starter code provided for model development and reference.
- `SMSSpamCollection.csv`: The dataset used for training the model, with labeled SMS messages.

## Dataset

The dataset `SMSSpamCollection.csv` contains labeled SMS text messages with the following columns:

- `label`: The classification of the message (`ham` for not spam, `spam` for spam).
- `text_message`: The actual content of the SMS message.

## Features

- Builds a machine learning pipeline using `TfidfVectorizer` and `LinearSVC`
- Splits data into training and testing sets with a test size of 33 percent
- Trains a model to classify messages as spam or not spam
- Provides a function for predicting the classification of new text messages
- Deploys a Gradio interface for real-time message classification

## Technologies Used

- Python
- Pandas
- Scikit-learn (TfidfVectorizer, LinearSVC, Pipeline)
- Gradio

## How It Works

1. The CSV file is loaded into a pandas DataFrame and cleaned by dropping missing values.
2. A classification function builds and trains a pipeline with TF-IDF vectorization and a linear SVC model.
3. A prediction function takes user input and classifies the message as "spam" or "not spam."
4. A Gradio interface is created to allow users to enter a message and see the result.

## Getting Started

1. Clone this repository to your local machine.
2. Install the required packages by running: pip install pandas scikit-learn gradio
3. Open and run `gradio_sms_text_classification.ipynb` in Jupyter Notebook or VS Code.
4. The Gradio app will launch with a public URL to share.

## Example Messages to Test

Use these example messages to test the application:

- You are a lucky winner of $5000!
- You won 2 free tickets to the Super Bowl.
- You won 2 free tickets to the Super Bowl. Text us to claim your prize.
- Thanks for registering. Text 4343 to receive free updates on medicare.

## License

This project was developed for educational purposes as part of a machine learning bootcamp assignment.
