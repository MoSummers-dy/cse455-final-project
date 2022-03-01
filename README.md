# CSE455 Final Project Proposal: Flower Classification on TPU
Date: 3/1/2022

## Group Members
Diana Dai, Alisa Shi

## Project Description
This project is from a Kaggle competition (https://www.kaggle.com/c/tpu-getting-started). There are a lot of species in nature, for over 5,000 species of mammals, 10,000 species of birds, and 30,000 species of fish. How about some plants? Well, we have over 400,000 different types of flowers! Incredible!

For this competition, each team is challenged to build a machine learning model that identifies the type of flowers in a dataset of images. The good news is, we will have just over 100 types, so the work is already easier.

## Algorithms / Techniques
There are several parts that make this project exciting. First of all, we will be using Tensor Processing Units (TPUs) that are provided in the Kaggle Notebook, instead of CPUs or GPUs. Our plan is to train with several different models and add in some augmentation on the data to see if a better accuracy can be achieved. We will use transfer learning, which is reusing part of a pre-trained model to get a head-start on a new dataset. If we have time, we might also explore the differences between training from scratch vs. transfer training.

## Dataset
The Kaggle competition provides data (https://www.kaggle.com/c/tpu-getting-started/data) in TFRecord format, which fits well into TPUs. We have:
* ```train/*.tfrec``` - training samples, including labels.
* ```val/*.tfrec``` - pre-split training samples w/ labels intended to help with checking your model's performance on TPU. The split was stratified across labels.
* ```test/*.tfrec``` - samples without labels - you'll be predicting what classes of flowers these fall into.
* ```sample_submission.csv``` - a sample submission file in the correct format

## Other Information
We will start with this tutorial notebook (https://www.kaggle.com/ryanholbrook/create-your-first-submission), which only trains the dataset with one model. Our goal is to try different models and try our best to reach high accuracy.

## Note
Our project may change as we start working on it. Please refer to our final product for what is accomplished.
