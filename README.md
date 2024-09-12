102117016_SESS_LE1

Activities Completed
Audio Sample Recording: Recorded 30 distinct audio samples, each containing 35 unique words, using a laptop's built-in voice recording software.

Dataset Assembly: Compiled all recorded audio samples into a zip file and uploaded it to Google Drive. The Drive was then mounted in the working environment, and the zip file was extracted to access the individual audio files for further processing.

Data Processing: Organized the extracted audio files for model training. Converted the audio to mono if necessary and resampled all files to 8000 Hz to ensure consistency.

Custom Dataset Class Creation: Designed a custom dataset class called MySpeechCommands to load and preprocess the audio data. This class includes methods to handle stereo-to-mono conversion, audio resampling, and label mapping to corresponding indices for training.

CNN Classifier Development: Built and configured a Convolutional Neural Network (CNN) named M5, designed for keyword spotting. The architecture includes multiple 1D convolutional layers, batch normalization, pooling, and a fully connected layer to classify audio inputs.

Data Splitting: Divided the dataset into training, validation, and testing sets using custom file lists to ensure a balanced and efficient distribution of samples for model evaluation.

Model Fine-Tuning: Fine-tuned the CNN model using the prepared dataset. After 10 epochs of training, the model achieved a validation accuracy of 0.8190.

Model Evaluation: Assessed the model's performance on a separate test set to evaluate how well it generalizes to unseen data. The initial test run resulted in an accuracy of 0.0286, indicating that further adjustments and debugging are required to improve performance

#CODE-LINK:https://colab.research.google.com/github/JasmineDas5/102117016_SESS_LE1/blob/main/about-lab-eval/102117016_Jasmine_Das.ipynb

