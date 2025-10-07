# char-level-lstm
A simple character-level LSTM text generator implemented in PyTorch. Trains on "The Making of a Marchioness" by Frances Hodgson Burnett and generates Victorian-era prose one character at a time.

# What it does
This is a basic LSTM that learns to predict the next character in a sequence. After training on classic literature, it can generate new text that mimics the style of the training data.

# Scale Factor (Temperature)
We experimented with different scale factors to control generation creativity:

0.5: Conservative, repetitive, sticks closely to learned patterns
1.0: Balanced sampling from the model's predictions
2.0: More creative and diverse, sometimes unexpected

Higher scale factors make the probability distribution flatter, leading to more diverse but potentially less coherent outputs.

#Model Architecture
- Embedding layer
- LSTM (2 layers, 256 hidden units)
- Fully connected output layer
