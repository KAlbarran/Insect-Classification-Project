# Insect-Classification-Project
For this project, a pretrained model is used to classify different images of pest insects & recognize what species they belong to. The goal is to train the model so it's able to recognize any species when given any image.

The dataset used is from HuggingFace. The pretrained model used is the EfficientNet-B1 model. To learn how to use these items, go to the "Project Dataset, Model, & Recording" md file.

First, the dataset is loaded with preexisting splits, each of which are reduced in number of images to make it easier to run program & weaker systems. Then, the data is given labels in case the ones in features were incorrectly formatted. After, images in training, validation, & testing splits are converted to PIL image format in case of any issues & then converted to tensor format. After, the number of batches is set to 32, epochs are set to 40 for less time training, & the model & optimizer (Adam) are initialized. THen the training & validation loop comences, training the data before the testing plase occurs. Finally, all results are gathered through metric calculations, accuracy & loss charts between training & validation, & a confusion matrix between the 15 biggest classes.

To run the code, you have two options: you can try to use the Jupyter Scource file & open it in a IDE that supports this format or use the python file & run every part of it at the saem time.

The only true depenedencies are the continued availability of the dataset withing the HuggingFace website, relying on GPU to run the code unless a stronger system is used, & which file format you are able to use in your given IDE.
