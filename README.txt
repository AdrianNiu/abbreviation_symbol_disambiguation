This folder contains the datasets and baseline models for homework 1 of HINF 5610. 

* README.txt: This file.
* abbreviation_disambiguation_baseline.py: The script for training and evaluating the baseline feature set
					   and model for the abbreviation and acronyms dataset.
* symbol_disambiguation_baseline.py: The script for training and evaluating the baseline feature set
				     and model for the symbols dataset.
* requirements.txt: External packages required by the above Python scripts.
* data/AbbreviationsDataSet.csv: The abbreviation and acronyms dataset.
* data/DeidentifedSymbolDataSet.csv: The symbols dataset.
* data/README_AbbreviationsDataSet.csv: A description of the abbreviation and acronyms dataset.
* data/README_DeidentifedSymbolDataSet.csv: A description of the symbols dataset.
* evaluation/abbreviation_baseline_evaluation.txt: The evaluation for the baseline abbreviation and acronyms disambiguation model.
* evaluation/symbol_baseline_evaluation.txt: The evaluation for the baseline symbol disambiguation model.


Run the baselines using the following commands:

python abbreviation_disambiguation_baseline.py data/AbbreviationsDataSet.csv evaluation/abbreviation_evaluation.txt

python symbol_disambiguation_baseline.py data/DeidentifedSymbolDataSet.csv evaluation/symbol_evaluation.txt
