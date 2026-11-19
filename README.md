# Amazon Review Sentiment Analysis

An educational Python project for analyzing product-review sentiment, comparing Naive Bayes and Random Forest after text preprocessing and TF-IDF feature extraction.

[Open in Google Colab](https://colab.research.google.com/github/eid-12/amazon-review-sentiment-analysis/blob/main/sentiment_analysis.ipynb)

## What the notebook covers

- Load review text and binary sentiment labels.
- Remove missing entries and duplicate reviews.
- Normalize text, remove URLs and punctuation, tokenize and stem words.
- Split training and test data before fitting the TF-IDF vocabulary.
- Compare Multinomial Naive Bayes and Random Forest with accuracy and confusion matrices.
- Try predictions on your own input.

## Run

Open the notebook with the Colab link, upload a permitted `Amazon-Product.csv` to the runtime, install the packages from `requirements.txt`, then run the cells in order. You can install them in a Colab code cell with `%pip install pandas numpy scikit-learn nltk matplotlib`.

The CSV must have `review_body` (English text) and `sentiment` (0 = negative, 1 = positive). Obtain data from its original provider and follow its terms. No dataset is redistributed here. A free CPU runtime is sufficient for the workflow, although Random Forest training can take time.

## About this export

This is a curated export of an existing Colab learning project. Unrelated Twitter exercises, stored outputs and runtime metadata were omitted. The vocabulary now fits only the training data, and duplicate removal is applied in place. The original Google Drive notebook was not changed.

Previous accuracy outputs are intentionally not presented as validated results of this version. Rerun with your dataset to obtain fresh metrics. Class imbalance can make accuracy misleading; compare against a majority-class baseline and inspect both classes in the confusion matrix. This notebook is an educational experiment and is not intended for production decisions.
