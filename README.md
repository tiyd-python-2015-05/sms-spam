# Classify and Cluster SMS Messages

## Description

Use Bayesian classification to analyze SMS messages.

## Objectives

### Learning Objectives

After completing this assignment, you should understand:

* The uses of classification and clustering
* Good feature extraction

### Performance Objectives

After completing this assignment, you should be able to:

* Parse text into features
* Classify textual data
* Cluster textual data

## Details

### Deliverables

* A Git repo called sms-spam containing at least:
  * `README.md` file explaining how to run your project
  * a `requirements.txt` file

### Requirements  

* No PEP8 or Pyflakes warnings or errors

## Normal Mode

Download the [SMS Spam collection](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) from the UCI Machine Learning Repository.

Choose a set of features to use in order to separate SMS ham from spam.

Write a program to extract the features you want from each SMS message and then classify each SMS as ham or spam. Iterate on your feature extraction until you
have a classification success level you are comfortable with (> 75% minimum.)

You may want to start with using `CountVectorizer` and then possibly build your
own feature extractor.

## Hard Mode

In addition to the requirements from **Normal Mode**:

Write your own feature extractor using the same interface as `CountVectorizer`
and other `scikit-learn` tools so you can include it in a Pipeline. Use a Pipeline
for your classifier. Bonus points if you can start from the raw text of the
SMSSpamCollection file without any processing outside of a pipeline.

## Notes

Some features you might want to try:

* Presence of the following words: claim, winner
* Presence of money symbols
* Presence of numbers
* Presence of first-person words

## Additional Resources

* [TextBlob](http://textblob.readthedocs.org/en/dev/)
* [Bag of Words model](https://en.wikipedia.org/wiki/Bag-of-words_model)
