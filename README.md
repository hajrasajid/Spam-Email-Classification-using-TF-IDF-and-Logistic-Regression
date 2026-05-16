# Spam Email Classification using TF-IDF and Logistic Regression

This project implements a spam email classification system using Natural Language Processing (NLP) and Machine Learning techniques.

## Dataset

* Total samples: 5734 emails
* Features:

  * `text`: email content
  * `spam`: binary target label (0 = not spam, 1 = spam)

## Data Preprocessing

The dataset was cleaned by:

* Removing missing values
* Removing duplicate records
* Converting labels into integer format
* Cleaning text using regular expressions:

  * lowercase conversion
  * punctuation removal
  * special character removal

## Feature Extraction

TF-IDF Vectorization was applied to convert text into numerical feature vectors.

## Model

Logistic Regression was used for classification.

## Results

* Train Accuracy: 99.52%
* Test Accuracy: 97.60%

### Classification Performance

* Precision (Spam): 1.00
* Recall (Spam): 0.91
* F1-Score (Spam): 0.95

### Confusion Matrix

```text
[[1267    2]
 [  39  400]]
```

Interpretation:

* 1267 non-spam emails were correctly classified.
* 400 spam emails were correctly detected.
* Only 2 normal emails were incorrectly classified as spam.
* 39 spam emails were missed by the model.

## Conclusion

The Logistic Regression model achieved high accuracy and strong spam detection performance with very few false predictions, making it an effective approach for email spam classification.

## Author Name
Hajira Sajid
