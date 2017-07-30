# Summarization evaluation by theta human judgements comparison.

This tool computes the correlations between a given theta and human judgements. 

A theta is a scoring function that takes as input a summary and a document collections and outputs
a score.

It needs as input a dataset of manual annotations with summary manual scored with pyramid and responsiveness scores. The tool computes the pearson's r, spearman's rho and NDCG@10 between the theta and the two manual annotations.

## Requirements
* Python 2.7
* Numpy 1.11.1 (http://www.numpy.org)
* nltk 3.2.1 (http://www.nltk.org)

## Usage

An example of theta is provided: jensen-shanon divergence between summary and the document collection.
Some sample data are also provided to show the structure that the tool expects.

In order to replace the sample data with a real dataset, the user should modify the following variables in the file read_data:
- MANUAL_ANNOTATIONS_FOLDER
- DATASET_FOLDER 

To test the installation just run:
python example.py

