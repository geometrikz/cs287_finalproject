# Code for Improving Robustness of Factual Abstractive Summarization viaRelation-Targeting Data Augmentation

This is the main folder containing the code for our project. There are 4 main folders which contain jupyter notebook scripts that generate the data, tain the model and evaluate the model. There is an extra folder with our sagemaker training script, however there are sagemaker account and instance dependent, so it is best to refer to 'offline_training' folder for scripts to train our model.

The four folders are:

* xsum_baseline: this contains the code to generate the baseline summaries using a pretrained BART-large model that is fine-tuned to the XSum dataaset available on Hugging Face

* generate_dataset: this contains the scripts to generate our corruptions as well as the baseline entity corruptions

* evaluation: This contains the script to evaluate our dataset.

* sagemaker_training: These are scripts specific to training and deploying our model on Sagemaker using Sagemaker's HuggingFace API.

* data: The data folder containing all our data used for the model can be accessed via https://drive.google.com/file/d/1_by5_bGmecM8wX-5elLBCuB5cj97U_Ep/view?usp=sharing


For ease of running, we provide jupyter notebooks to run our code instead of python files. All the packages required are the latest package versions as of 12/1/2021, and all packages required to run each of our scripts is imported in each jupyter notebook.

This list of packages required is (based off their PyPI names):

* torch
* transformers
* dataclasses
* numpy
* pandas
* nltk
* rouge_score
* spacy
* stanza
* tqdm
* matplotlib
* googletrans
* pyinflect

We also used sagemaker specific packages and google colab specific packages that cannot be installed via PyPI, however these were mainly to set data directories to S3 buckets or Google Drive buckets. These parts of the code can be commented out if running our codebase locally.