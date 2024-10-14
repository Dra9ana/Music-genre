# Audio Classification Project Using GTZAN Dataset

## Overview

This project focuses on classifying music genres using audio feature extraction methods applied to the GTZAN dataset, which consists of ten music genres, each containing 100 audio samples of 30 seconds each. The primary goal of the project is to explore the impact of different audio features on classification performance and to implement a sequential model using Long Short-Term Memory (LSTM) layers for the classification task.

## Project Objectives

- To analyze and preprocess audio data for effective feature extraction.
- To implement various audio feature extraction techniques, including Short-Time Fourier Transform (STFT), Mel-frequency cepstral coefficients (MFCC), zero crossing rate, and chroma features.
- To develop and evaluate a sequential LSTM model for music genre classification.
- To assess the impact of different audio features on classification accuracy.

### Dataset

The GTZAN dataset is publicly available and contains a diverse range of music genres, including:

- Blues
- Classical
- Country
- Disco
- Hip-Hop
- Jazz
- Metal
- Pop
- Reggae
- Rock

Each genre consists of 100 audio samples, with each sample lasting 30 seconds.

### Data Preprocessing

1. **Audio Segmentation**: The audio samples were divided into smaller segments to facilitate feature extraction.
2. **Balancing the Dataset**: Ensured that each genre was represented equally in the training set to avoid bias.
3. **Standardization**: Applied normalization techniques to standardize the audio features across different genres.

### Feature Extraction

The following audio features were extracted for classification:

- **Short-Time Fourier Transform (STFT)**: Used to analyze the frequency content of audio signals over time.
- **Mel-frequency cepstral coefficients (MFCC)**: Captured the short-term power spectrum of sound, commonly used in speech and audio processing.
- **Zero Crossing Rate**: Measured the rate at which the audio signal changes sign, which is useful for detecting the noisiness of the signal.
- **Chroma Features**: Represented the energy distribution across different pitch classes, useful for identifying harmonic structures.

### Model Development

- **Sequential LSTM Model**: 
  - Implemented a deep learning model using Keras with LSTM layers to capture temporal dependencies in the audio data.
  - Optimized the model parameters using a hold-out validation method to ensure unbiased estimation.

### Evaluation

- **Metrics**: Used accuracy, precision, recall, and F1-score to evaluate the performance of the classifier.
- **Confusion Matrix**: Generated confusion matrices to visualize the classification performance across different genres.

## Results

The classification model demonstrated promising results, with an overall accuracy of **86.64%** on the validation set. The performance varied across different genres, highlighting the model's strengths in recognizing certain genres over others. 

### Key Findings

- Certain audio features, such as MFCC and chroma features, significantly improved the model's performance compared to others.
- The LSTM model effectively captured the sequential nature of audio signals, leading to better classification accuracy compared to traditional classifiers.

## Achievements

- Successfully implemented audio feature extraction methods that enhanced model performance.
- Developed a robust sequential model using LSTM layers for music genre classification.
- Gained insights into the significance of different audio features in the classification task, which can inform future research and development in audio processing and machine learning.

## Conclusion

This project highlights the potential of deep learning techniques, specifically LSTM networks, in the field of audio classification. The findings provide a foundation for future exploration of more complex models and additional audio features that can further enhance classification accuracy.

## References

- GTZAN Dataset: [GTZAN Music Genre Dataset](http://marsyas.info/downloads/datasets/)
