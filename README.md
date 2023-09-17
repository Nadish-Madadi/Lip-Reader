# Lip Reading CNN-LSTM Model

- Utilized TensorFlow, Keras, OpenCV, Matplotlib, and gdown to create a deep neural network with Conv3D and LSTM layers, designed for video and text sequence analysis (lip reading)

## Key Features

- **Spatiotemporal Feature Extraction:** Utilize Conv3D layers to capture spatiotemporal patterns in lip movement across video frames.
- **Sequential Modeling:** Employ Bidirectional LSTM layers to model sequential dependencies in the video data.
- **Connectionist Temporal Classification (CTC) Loss:** Implement CTC loss to align video frames with transcribed text, improving speech recognition.
- **Feature Aggregation:** Use Dense layers to aggregate and transform extracted features for accurate predictions.
- **Overfitting Prevention:** Apply Spatial Dropout to prevent overfitting and enhance model generalization.

## Layers in Detail

1. **Conv3D (Convolutional 3D) Layers:** In the lip reading project, Conv3D layers were employed to extract spatiotemporal features from the video data. This allowed the network to analyze both spatial and temporal information in lip movement across frames, enhancing its ability to recognize spoken words.

2. **Bidirectional LSTM (Long Short-Term Memory) Layers:** Bidirectional LSTM layers were strategically integrated to model sequential dependencies in the video data. By processing frames bidirectionally, the network considered context from past and future frames, capturing dynamic lip movements and improving text prediction.

3. **Dense Layers:** Dense layers were used for feature aggregation and transformation. After extracting features with Conv3D and modeling sequences with Bidirectional LSTM layers, Dense layers processed these features to make predictions, connecting learned representations to the final output.

4. **Flatten Layer:** The Flatten layer played a key role in preparing data for the Dense layers by converting multidimensional output into a one-dimensional format, facilitating feature aggregation and decision-making.

5. **Spatial Dropout:** Spatial Dropout was applied within Conv3D layers to prevent overfitting. By deactivating entire feature maps during training, the model avoided overreliance on specific features, promoting generalization and robustness in recognizing various lip movements and speech patterns.

In summary, the use of these layers assisted in effective video data processing, sequential modeling, feature aggregation, and overfitting prevention, resulting in improved speech recognition for the hearing-impaired community.
