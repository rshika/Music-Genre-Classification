# Music-Genre-Classification
This project categories music based on genre.The dataset used here is GTZAN datset, an universal dataset for music related projects, the link for the dataset is given below. The raw data is preprocessed and trained to get the desired output. ML and DL can be used for the better accuracy of the project.
Raw data:
Download GTZAN Dataset from: http://opihi.cs.uvic.ca/sound/genres.tar.gz Raw data is 1.2GB and consists of 1000 audio files(.au) divided into 10 folders for 10 genres equally. I.e Every genre has 100 audio files.

Preprocessed data
The raw audio has been converted to mel-spectograms and other features using librosa library for Machine Learning purpose and can be found in the folder as csv file. Feature spectrogram images are made from the audio files directly during training for Deep Learning model.

Code Notebooks
Machine Learning
To run code in any of these notebooks, first please download raw data from Dataset link above

make_dataset_ml: Extracts features from dataset for ML training.
audio_data_visualization: Plots time series visualization and spectograms for the 10 different genres and exports them as image.
train_classical_ml_models: Loads the generated feature file. Trains the dataset using lgbm+SVM and XGBoost architecture and exports the model after training.
Deep Learning
CNN_train: This notebook contains all the steps right from creating images from audio to training them using CNN and finally exporting the model too
Conclusion
Deep Learning methodology proves to be more accurate with around 75% accuracy in classifying the genres whereas machine learning acheives around 65% accuracy. You can see the csv file in models directory where the comparison is made between used architectures.
