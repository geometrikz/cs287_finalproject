# Offline Model Training Scripts

This folder contains scripts to train our factual corrector model offline.

* BART_baseline: trains the baseline model with entity swaps only
* BART_predicate: trains our model with relation and predicate swaps.

These two python files use our dataset which is uploaded seperately, 

* the BART_baseline file calls data from "data/xsum_corrupted_entity_untokenized"
* the BART_predicate model file calls data from "data/xsum_corrupted_predicate_untokenized/train"

Checkpoints are saved into the "exp" folder, these are available upon request due to their large file sizes.