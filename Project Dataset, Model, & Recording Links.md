Presentation Recording
<br>
Link: https://drive.google.com/file/d/1qRIB6S85Y6__QCzfuUVMmaDOAhPW5M-4/view?usp=sharing
<br>
<br>
<br>
Project Dataset
<br>
This data set came from the EnmmmmOvO/insect-pest-dataset in HuggingFace.
<br>
Link: https://huggingface.co/datasets/EnmmmmOvO/insect-pest-dataset
<br>
<br>
It contains 75,000 images, most which originated from the IP102 dataset.
<br>
This file can be downloaded from its GitHub Repository.
<br>
Repository Link: https://github.com/xpwu95/IP102
<br>
<br>
To use, write in a python file to load the dataset:
<br>
from datasets import load_dataset
<br>
ds = load_dataset("EnmmmmOvO/insect-pest-dataset")
<br>
<br>
<br>
Project Model Used
<br>
This project used the EfficientNet-B1 pretrained model made by Google.
<br>
Learn more about it: https://huggingface.co/google/efficientnet-b1
<br>
Basic Setup: 
<br>
from transformers import AutoImageProcessor, AutoModelForImageClassification # in case other models used
<br>
processor = AutoImageProcessor.from_pretrained("google/efficientnet-b1", size={"height": 128, "width": 128})
<br>
model = AutoModelForImageClassification.from_pretrained("google/efficientnet-b1",num_labels=num_classes, ignore_mismatched_sizes=True) # auto as model changes common
