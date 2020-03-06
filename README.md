# CNNFaceRecognition
Built a CNN Model which recognizes people in videos.

The video-based Datased used is private and cannot be uploaded.

# VideoProcessing
Videos have been processed in Video Stream.ipynb and person33.ipynb (person33 required a different approach to be identified). Two haarcascade xml files were used to detect faces in each frame, the first one to actually detect them, the second to discard which one was not a face.

# Folders structure
All the videos used contained 7 subjects. For each video we extracted the face of each subject in a folder named with the selected subject's unique id. This was done for labeling purposes.

# CNN Training, validation and testing
This is contained in Train-Validation-Testing.ipynb
We managed single 3-d image data in order to fit CNN and then we used them to train and validate the model.
The accuracy was 99% on training, 95% on validation and 86% on test.
Test set was completely isolated, during the training session test set example have not been taken under consideration.
For each item in test set we printed out a csv file containing actual and predicted value.

In the repository you can find the main plots.

# SAVING TRAINED MODEL
This is contained in Train-Validation-Testing.ipynb
We saved trained model in files

# USING SAVED MODEL TO PREDICT
This is contained in PredictionModule.ipynb
We load the best model and use it to make predictions on single files.
