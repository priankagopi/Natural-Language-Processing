# Sentiment Classification using IMDB Movie Reviews Dataset
This project focuses on sentiment classification using the IMDb movie reviews dataset. The goal is to classify movie reviews as positive or negative based on their sentiment.

## Dataset Overview
The IMDb movie reviews dataset contains a total of 50,000 movie reviews, with 25,000 reviews for training and 25,000 for testing. The reviews are labeled as positive or negative and are stored as text files within the "train" and "test" folders. The dataset has been preprocessed to remove unnecessary elements such as HTML symbols, emoji representations, numbers, punctuation, and stopwords.

## Model Architecture
For sentiment classification, a pre-trained DistilBERT model is utilized as a transformer model. A classification layer is added on top of the DistilBERT model to create a Keras model. The model is trained on the training data for 3 epochs using an Adam optimizer and binary cross-entropy loss function.

## Results
The model's performance is evaluated on the test data using various metrics. The overall accuracy of the model's predictions on the test set was found to be 84%. The classification report provides additional details, including precision, recall, and F1-score for each class (positive and negative). The model demonstrates balanced performance across both classes, indicating its ability to classify sentiments effectively.

## Usage
To reproduce the sentiment classification task using this project, follow these steps:

Clone the repository: git clone https://github.com/priankagopi/Natural-Language-Processing.git \
Install the required dependencies: pip install -r requirements.txt \
Execute the script or notebook for data preprocessing and model training. \
Evaluate the model's performance on the test set and generate the classification report. \
Modify the code as needed for further experimentation or fine-tuning.

## Conclusion
The accuracy of the linear probed model yielded a value of 87.86% as opposed to 84% without linear probing. The project demonstrates the effectiveness of pre-trained transformer models like DistilBERT for sentiment analysis tasks. The provided code and documentation can be used as a starting point for similar sentiment classification projects or further research in NLP.
