# Anomaly-Detection-with-LSTM-Autoencoder

As part of my research and experimentation, I've developed a robust anomaly detection system tailored for time-series data. Anomalies in such data can be critical indicators of irregularities, system failures, or other noteworthy events. My approach involves the implementation of an LSTM-based Autoencoder model, designed to effectively capture and identify these anomalies.

Here's a technical breakdown of what I've accomplished:

**Data Preparation:** To ensure the model's effectiveness, I've meticulously prepared the time-series data. I've segmented it into sequences of fixed time-steps, ensuring that temporal dependencies are preserved and available for model training.

The Graph representing JPMC Stock prices over 23 years:-
![image](https://github.com/Soumya-Panda/Anomaly-Detection-with-LSTM-Autoencoder/assets/81625214/c77ebad4-575a-4f85-a2ab-02e1ea2feafa)

**Autoencoder Architecture:** My Autoencoder architecture is a key component of this project. It employs LSTM layers for their ability to capture temporal patterns. Additionally, I've incorporated Dropout layers for regularization, reducing the risk of overfitting, and TimeDistributed Dense layers to facilitate data reconstruction.

![image](https://github.com/Soumya-Panda/Anomaly-Detection-with-LSTM-Autoencoder/assets/81625214/f4039000-8bd8-46f2-9b45-04b0b5772e09)

**Training Strategy:** I've trained the model over a specified number of epochs, utilizing the Adam optimizer and mean squared error (MSE) loss function. The batch size used during training has been optimized to suit the dataset's characteristics.

**Anomaly Detection:** Post-training, I've employed a threshold-based approach to detect anomalies. By comparing the Mean Absolute Error (MAE) of test data with the maximum training MAE, I can effectively identify anomalies in the time-series.

![image](https://github.com/Soumya-Panda/Anomaly-Detection-with-LSTM-Autoencoder/assets/81625214/5de9489f-ffe5-437e-b29d-1dc75c4b9a7e)

**Visualization:** I've included code for visualizing the identified anomalies within the original data. This visualization aids in gaining a deeper understanding of the detected anomalies' context and significance.

![image](https://github.com/Soumya-Panda/Anomaly-Detection-with-LSTM-Autoencoder/assets/81625214/56933519-1179-42ae-be03-7c291b6ada86)
The **Red** areas show anomalies on the data

This repository serves as a comprehensive technical guide for implementing and applying this LSTM-based Autoencoder approach to time-series anomaly detection, showcasing the results of my dedicated research and experimentation in this domain.
