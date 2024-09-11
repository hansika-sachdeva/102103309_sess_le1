# 102103309_sess_le1 REPORT

# About the research paper

The Speech Commands dataset is an open-source resource created to assist in the development and evaluation of keyword spotting systems. Its primary purpose is to facilitate the creation and testing of small models that can accurately detect specific spoken words from a set of ten or fewer target words while reducing false positives from background noise or unrelated speech. By standardizing model comparisons, this dataset plays a crucial role in advancing the field and promoting collaborative research.

The dataset enables meaningful evaluations of different models’ ability to distinguish between speech-containing audio clips and non-speech clips. With Version 2, the dataset shows significant accuracy improvements, achieving a top-one score of 88.2% on the training set and 89.7% on the Version 1 test set. Unlike general speech datasets like Mozilla’s Common Voice, which support various speech tasks, the Speech Commands dataset is specifically tailored to keyword spotting. This specialization allows it to focus on testing and building on-device models, ensuring reproducibility and comparable performance metrics across baseline models. It remains a valuable resource for training and evaluating various models, with Version 2 demonstrating better performance than the original dataset on similar test data.

The dataset was gathered using an open-source, web-based application that utilized the Web Audio API to record short utterances of words from a predefined list. This user-friendly application helped minimize recording failures. Each recording was processed to remove quiet segments and isolate the loudest part of the clip. A default convolutional model from TensorFlow’s tutorial was trained on both Version 1 and Version 2 data, and the resulting models were evaluated on their respective test sets.

# Activities Completed
Recording Audio Samples:
Recorded 30 audio samples, each containing 35 distinct words. Used a laptop voice recorder for capturing the audio.

# Dataset Preparation:
Compiled the recorded audio samples into a zip archive. Uploaded the zip file to the working environment. Extracted the zip file to access the individual audio files for processing.

# Data Extraction:
Extracted the dataset from the zip file to a specified directory. Ensured the audio files were ready for model training by organizing and processing them.

# CNN Model Classifier Development:
Selected and implemented a Convolutional Neural Network (CNN) model for the keyword spotting task. Configured the CNN model to work with the extracted audio dataset achieving accuracy of 73%.

# Dataset Splitting:
Prepared the dataset for training and testing. Planned to split the dataset into training and testing subsets to evaluate the model’s performance.

# Fine-Tuning Process:
Initiated the fine-tuning of the CNN model using the prepared dataset. Applied training data to optimize the model for keyword detection.

Challenges Encountered:
Faced limitations due to lack of GPU resources, affecting the ability to complete and optimize the model training process. Unable to fully fine-tune the model and apply necessary corrections due to computational and time constraints.

# Snapshots
![Screenshot (209)](https://github.com/user-attachments/assets/922e450d-8ba5-4841-9ca0-34c74ea4d91a)

### Model Architecture
![Screenshot (209)](https://github.com/user-attachments/assets/7a80b534-5b3f-4178-a203-53527ee10993)

### Training and Testing Model
![Screenshot (210)](https://github.com/user-attachments/assets/55d65fbf-b88a-42eb-b0f0-54b4fed7640d)
![Screenshot (211)](https://github.com/user-attachments/assets/d1375151-fb66-49ef-88d3-292b2dc2ec43)

### Training Loss
![Screenshot (213)](https://github.com/user-attachments/assets/ce0c2959-b852-4d14-9862-82ff03f228b4)

![Screenshot (212)](https://github.com/user-attachments/assets/66755eeb-6d82-4220-80bd-cc3e9e6eb230)




