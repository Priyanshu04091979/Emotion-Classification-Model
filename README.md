# -Emotion-Classification-Model

This project implements a text-based emotion classification model that detects emotions from user-inputted text (e.g., happy, sad, angry).

1.Dataset Used
  Dataset: Emotion Dataset 
    6 basic emotions: joy, sadness, anger, fear, surprise, love
    Format: CSV with text and emotion columns
    Total samples: ~34,000
2. Approach Summary
    Text Preprocessing
      Clean text (lowercase, remove punctuation/special characters).
      Tokenize and convert words to sequences.
      Pad sequences to a uniform length.
    Feature Representation
      Use word embeddings (e.g., Embedding layer or pre-trained like GloVe/BERT) to represent text in vector form.
    Model Architecture
      Option 1 (Basic):
      Embedding → LSTM / BiLSTM → Dense → Softmax
      Option 2 (Advanced):
      Pre-trained Transformer (e.g., BERT) + classification head
    Training
      Categorical crossentropy loss function.
    Prediction
        Input new user text → preprocess → predict emotion label.
3. Dependencies
    Install via requirements.txt:
    pip install -r requirements.txt
    Main packages:
      pandas
      numpy
      scikit-learn
      joblib
      streamlit

