# Spam Classification

Binary classifier (spam vs. ham) for SMS messages using Multinomial Naive 
Bayes with bag-of-words features.

**Approach:** Preprocessed text (lowercasing, stopword removal, stemming), 
then vectorized with `CountVectorizer` (unigrams + bigrams). Used 
`GridSearchCV` to tune the Laplace smoothing parameter (`alpha`) via 
5-fold cross-validation, optimizing for F1-score.

**Dataset:** [SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection) 
(5,574 labeled SMS messages)

**Result:** ~91% accuracy on held-out evaluation data.
