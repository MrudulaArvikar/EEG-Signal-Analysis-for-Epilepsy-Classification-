# EEG-Signal-Analysis-for-Epilepsy-Classification-

**Installation**
To get started, install the MNE package, which is used for analyzing EEG data.

**Download Data**
The dataset used in this project was collected using the EMOTIVE system with a 128 Hz sampling frequency. Two datasets were collected: one in Guinea-Bissau (97 subjects) and one in Nigeria (112 subjects). This project utilizes the Guinea-Bissau dataset.

You can download the dataset from Zenodo.

**Data Preparation**
Unzip the Data: Extract the downloaded zip file to access the data files.
Load Metadata: The metadata file contains information about the subjects and their group classifications (Epilepsy or Control).
Preprocess Data: The dataset includes EEG signals in CSV files. Each file is processed to remove non-EEG channels and convert the data into a format compatible with MNE.
Data Processing
Convert Data: Convert the preprocessed CSV files into MNE objects, which are then filtered and segmented into epochs.
Concatenate Epochs: Combine epochs from different subjects into a single dataset.
Create Labels: Label the epochs as belonging to either the Epilepsy or Control group.
Feature Extraction
The features used for classification are based on the power spectral density (PSD) of the EEG signals. The PSD is computed for different frequency bands (delta, theta, alpha, sigma, beta, gamma) to capture the frequency content of the EEG signals.

**Classification**
The classification task involves distinguishing between Epilepsy and Control subjects. A Random Forest Classifier is used for this purpose, with performance evaluated using 5-fold cross-validation. The average accuracy of the classifier is reported.

## Results

- **Accuracy Score**: Shows the percentage of correctly classified articles.
- **Confusion Matrix**: Visual representation of true vs. predicted labels.
- **Classification Report**: Includes precision, recall, and F1-score metrics.


Tips for Improvement
Experiment with different classifiers.
Tune the parameters of classifiers.
Try feature elimination to improve model performance.
Acknowledgments
This project is based on work originally developed by an unnamed source. If you recognize this work or have more information about the original author, please let me know so that proper credit can be given.
