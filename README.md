# NLU_Chatbot
A shopping chatbot that responds after intent extraction from user query by text classification.

Three implementation variations of the chatbot are presented in this project.

Creating Embedddings variations:
1. Word-level One-Hot-Encoded embeddings describing patterns and predicted intents respectively.
2. Sentence embeddings generated by SentenceTransformer model.

Classification variations:
1. Feed Forward Neural Network (NN) with forward pass layer weights optimization by Stochastic Gradient Descent and standard learning rate of 0.01. The NN uses ReLu activation function between outputs and inputs of adjacent hidden layers. Softmax is applied at the last layer to normalize the output layer results.
2. Cosine Similarity Function to pick intents embeddings most similar to the input query embedding.

The implementation variations are presented in the following directories:
1. word_classifier : uses One Hot Encoding for creating embeddings + Feed Forward NN for training intent classification model.

2. sentence_classifier: uses sentence embeddings by SentenceTransformer model + Feed Forward NN for training intent classification model.

3. sentence_cosine: uses sentence embeddings by SentenceTransformer model + cosine similarity to pick most intent embedding closest to query embedding.
