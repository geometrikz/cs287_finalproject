# Code for Improving Robustness of Factual Abstractive Summarization viaRelation-Targeting Data Augmentation

This is the main folder containing the code for our project. There are 4 main folders which contain jupyter notebook scripts that generate the data, tain the model and evaluate the model. There is an extra folder with our sagemaker training script, however there are sagemaker account and instance dependent, so it is best to refer to 'offline_training' folder for scripts to train our model.

The four folders are:

* xsum_baseline: this contains the code to generate the baseline summaries using a pretrained BART-large model that is fine-tuned to the XSum dataaset available on Hugging Face

* generate_dataset: this contains the scripts to generate our corruptions as well as the baseline entity corruptions

* evaluation: This contains the script to evaluate our dataset.

* sagemaker_training: These are scripts specific to training and deploying our model on Sagemaker using Sagemaker's HuggingFace API.

* data: The data folder containing all our data used for the model can be accessed via https://drive.google.com/file/d/1_by5_bGmecM8wX-5elLBCuB5cj97U_Ep/view?usp=sharing