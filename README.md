This is a News classifier with Bidirectional RNN model and Bidirectional RNN with Attention model.

Data Preparation
  * Tokenize the text.
  * Reformat or Clean up some mal-formatted data.
  * Build a map from category to int and reversed index from an int to category.
  * Split the dataset to 80% train, 10% dev and 10% test.
  
Training Process
For each epoch:
  * Embedding layer uses GloVe for word embedding.
  * Bidirectional RNN layer uses Tensorflow BasicLSTMCell with DropoutWrapper.
  * The output layer is a fully connected layer with softmax output.
  * The loss is calculated against labelled category and minimized with Adam Optimizer.

