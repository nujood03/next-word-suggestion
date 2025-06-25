# Next Word Suggestion System (LSTM-based NLP Project)

A basic NLP project using deep learning to predict the next word in a sentence.  
This model was trained on *Pride and Prejudice* by Jane Austen using a custom LSTM neural network built with TensorFlow and Keras.


## Project Overview

The purpose of this project is to learn and implement text preprocessing, tokenization, sequence generation, and train a deep learning model to predict the next likely word given the last 3 words in a sentence.



## Technologies & Tools

- Python
- TensorFlow / Keras
- Numpy
- NLTK
- Pickle
- Google Colab (for training)
- Project Gutenberg text corpus



##  Dataset

- **Source**: [Pride and Prejudice – Project Gutenberg](https://www.gutenberg.org/ebooks/1342)
- The full text was cleaned, tokenized, and used to train an n-gram + LSTM model.



##  Key Steps

1. **Text Preprocessing**
   - Removed special characters and newlines
   - Joined all text into a single string
2. **Tokenization**
   - Converted text to sequences using `Tokenizer`
3. **Sequence Creation**
   - Generated n-gram sequences with sliding windows of size 4
   - Split into input (`X`) and target (`y`)
4. **Model Building**
   - LSTM layers with embedding and dense layers
   - Output layer with softmax over vocabulary
5. **Training**
   - Trained for 7 epochs using categorical crossentropy
   - Used model checkpointing to save the best model
6. **Prediction**
   - Custom function to predict the next word based on user input (last 3 words)


