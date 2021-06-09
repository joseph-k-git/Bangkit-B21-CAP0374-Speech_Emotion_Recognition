# Bangkit-B21-CAP0374-Speech_Emotion_Recognition

1. SER directory is the saved trained model.
2. SER.tflite is also the saved trained model in TensorFlow Lite format.
3. Speech_Emotion_Recognition is the Python Notebook contains all the codes from Dataset Preprocessing, Model Building, Model Training, and Model Saving.

You can download the Audio_Speech_Actors_01-24.zip part of RAVDESS dataset and read more about it from https://zenodo.org/record/1188976
Extract Audio_Speech_Actors_01-24.zip into a folder (can be named Zenodo_1188976)

In the Speech_Emotion_Recognition.ipynb, change the data_path (the path of the folder that contains the extracted dataset) and json_path (the path of json file that contains the mfcc and labels) according to your need.
You can tweak the dataset preprocessing, for example: changing the splitting duration per segments, noise amplitude, audio sample rate, number of mfcc coefficient, mfcc time frame, and more.
If you change the segment duration, sample rate, number of mfcc coefficient, mfcc timeframe, and more, then usually the input size of the model should be changed.
You can tweak the model, for example: adding or removing layers, change number of nodes, change number of convolution filters, and more.
You can train the model in number of epochs you want. Based of my experience it's usually around 25 to 35 epochs.
Adjust the path where you want to save the model.
