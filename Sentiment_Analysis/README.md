# Sentiment Analysis

Binary sentiment classifier (positive/negative) for IMDB movie reviews: 
a skills-assessment exercise applying the spam-classification pipeline 
to a new dataset and problem.

**Approach:** Same core pattern as the spam classifier: `TfidfVectorizer`
feeding into Multinomial Naive Bayes, tuned via `GridSearchCV` over the smoothing parameter. The 
interesting part here isn't the technique itself but the transfer,
spam detection and sentiment analysis are both just text classification 
under the hood, and the same handful of preprocessing and modeling 
choices carry over directly.

**Dataset:** [IMDB Movie Review Dataset](http://www.aclweb.org/anthology/P11-1015) 
(Maas et al., 2011) — 25,000 labeled reviews

**Result:** Strong accuracy on the evaluation set; notably, this same 
pipeline generalizes to other text-moderation-style classification tasks 
beyond sentiment specifically.
