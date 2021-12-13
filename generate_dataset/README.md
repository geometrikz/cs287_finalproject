This folder creates scripts for creating out perturbed dataset.

* create_new_perturbations: creates the corruptions for both the baseline models presented in Cao et. al. 2020 and our model, and saves it to a folder named data.
* create_perturbed_dataset: adds perturbed summaries to the XSum dataset
* filter_data: filters the XSum data as per https://github.com/amazon-research/fact-check-summarization. We use a smaller subset of the data to train our model to save time the XSUM document id's we keep are recorded in data/ids_to_keep.npy

Our perturbations use CoreNLP for OpenIE implementation, which requires JAVA to be installed on the operating system.