Project Dataset
This data set came from the EnmmmmOvO/insect-pest-dataset in HuggingFace.
Link: https://huggingface.co/datasets/EnmmmmOvO/insect-pest-dataset

It contains 75,000 images, most which originated from the IP102 dataset.
THis file can be downloaded from its GitHub Repository.
Repository Link: https://github.com/xpwu95/IP102


To use, write in a python file to load the dataset:
from datasets import load_dataset
ds = load_dataset("EnmmmmOvO/insect-pest-dataset")
