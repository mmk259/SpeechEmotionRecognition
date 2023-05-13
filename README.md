# SpeechEmotionRecognition
_________________________________________________________________________________

# Introduction:
In this project, you are using the Toronto Emotional Speech Set (TESS) dataset to build a speech emotion recognition system. The TESS dataset contains audio recordings of actors speaking various sentences with different emotions, including anger, disgust, fear, happiness, neutral, and sadness. Your goal is to develop a machine learning model that can accurately predict the emotional state of a person based on their speech.


# Data Preprocessing:
To prepare the data for training, you first load the TESS dataset using the librosa library. You then extract various features from each audio sample, including the mel-frequency cepstral coefficients (MFCCs), chroma features, and spectral contrast. These features are commonly used in speech recognition tasks and help to capture different aspects of the audio signal.


# Model Architecture:
You use a convolutional neural network (CNN) to classify the emotional state of each audio sample. The CNN consists of multiple convolutional layers followed by pooling layers and a fully connected layer. The input to the network is the feature matrix extracted from the audio samples, and the output is a probability distribution over the different emotions. You use the categorical cross-entropy loss function to train the model and the Adam optimizer to update the network weights.


# Training and Evaluation:
You split the TESS dataset into training, validation, and test sets, with 80%, 10%, and 10% of the data allocated to each set, respectively. You train the CNN on the training set for a fixed number of epochs and monitor the accuracy and loss on the validation set to prevent overfitting. Once the model has converged, you evaluate its performance on the test set and report the overall accuracy as well as the precision, recall, and F1 score for each emotion.


# Conclusion:
In summary, you have developed a speech emotion recognition system using the TESS dataset and a convolutional neural network. Your model achieved a high accuracy on the test set, indicating that it can accurately predict the emotional state of a person based on their speech. This system could be useful in various applications, such as customer service chatbots, mental health monitoring, and speech therapy.
