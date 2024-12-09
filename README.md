# Sentiment-Analysis-of-Tweets
Classification of Tweets in three Sentiments -Negative,Positive,Neutral

This project analyzes Twitter sentiments using three different approaches: SVM, BiLSTM, and DistilBERT. Each model classifies tweets as negative (-1), neutral (0), or positive (1).
Setting Up Your Kaggle Environment
First, create a new notebook in Kaggle:

Go to kaggle.com and sign in
Click "Create" and select "New Notebook"
Click "Settings" on the right sidebar
Under "Accelerator," select "GPU T4 x2"
Save your settings

Running the Models
Support Vector Machine (SVM)
Create a new code cell and paste the SVM code. This model performs basic sentiment analysis using traditional machine learning. The code includes preprocessing steps like removing URLs, handling contractions, and converting text to TF-IDF features. Run time is approximately 10-15 minutes.
BiLSTM Model
For the BiLSTM implementation, create a new code cell and paste the BiLSTM code. This deep learning approach uses bidirectional LSTM layers to understand context in both directions. The model trains for 10 epochs and typically takes 30-40 minutes to complete.
DistilBERT Model
The DistilBERT implementation uses the transformers library. Create a new code cell and paste the DistilBERT code. This transformer-based model usually achieves the highest accuracy. Training runs for 3 epochs and takes about 90 minutes.
Performance Results
Each model achieves different accuracy levels:

SVM: 88% accuracy
BiLSTM: 96.93% accuracy
DistilBERT: 97% accuracy

Important Notes

Upload your dataset (train3.csv) to the Kaggle notebook
Keep the GPU sessions active while training
Save your outputs regularly
If you encounter memory issues, reduce batch sizes:

BiLSTM: Try batch_size=32
DistilBERT: Try batch_size=16
