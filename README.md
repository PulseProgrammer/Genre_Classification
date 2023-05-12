# Genre Classification using Mel Spectrograms and CRNN Architecture

This repository contains code for Genre Classification, focusing on utilizing Mel Spectrograms and a CRNN (Convolutional Recurrent Neural Network) architecture. The goal is to automatically classify music tracks into different genres using the GTZAN dataset, which consists of 10 genre classes.

## Introduction

Genre classification plays a vital role in various music-related applications, such as music recommendation systems, playlist generation, and content organization. This project aims to develop an accurate genre classification algorithm by leveraging Mel Spectrograms as a feature representation and employing a CRNN architecture for modeling the audio data.

## Implementation

The implementation involves the following steps:

1. Data preprocessing: The audio data from the GTZAN dataset is processed to generate Mel Spectrograms. Mel Spectrograms are two-dimensional representations that capture the frequency content of the audio signal over time. This involves segmenting the audio files into smaller frames, applying the Short-Time Fourier Transform (STFT) to obtain the magnitude spectrogram, and converting the magnitude spectrogram to a Mel scale.

2. Feature representation: The generated Mel Spectrograms serve as input features for the genre classification model. These spectrograms effectively capture the timbral characteristics of music tracks and are commonly used in audio-related tasks.

3. Model architecture: The genre classification model is built using a CRNN architecture. The CRNN combines convolutional layers to capture local patterns in the spectrograms and recurrent layers to capture temporal dependencies in the music sequences. This architecture has proven to be effective in handling sequential data like audio.

4. Model training: The model is trained using the GTZAN dataset, which provides labeled audio samples for each genre class. The training process involves feeding the Mel Spectrograms into the CRNN model and optimizing the model's parameters using techniques like backpropagation and gradient descent. The dataset is typically split into training and validation sets to monitor the model's performance during training.

5. Prediction: Once the model is trained and evaluated, it can be used to predict the genre of new, unseen music tracks by converting their audio data into Mel Spectrograms and feeding them into the trained CRNN model.

## Usage

To use the genre classification algorithm, follow these steps:

1. Set up a Google Colab environment and import the provided notebook.

2. Download the GTZAN dataset and ensure it is properly organized and accessible within the notebook environment.

3. Run the notebook cells step by step, following the provided instructions and code comments.

4. Train the CRNN model on the Mel Spectrograms, monitor the training progress, and evaluate the model's performance.

5. Use the trained model to predict the genre of new, unseen music tracks by following the prediction section in the notebook.

For detailed instructions, code examples, and explanations, please refer to the provided Google Colab notebook.

## Contribution

Contributions to this project are welcome. If you would like to contribute, please follow the code style guidelines and submit a pull request with your changes. Feel free to address any open issues or suggest improvements.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use the code for academic, research, or commercial purposes.

