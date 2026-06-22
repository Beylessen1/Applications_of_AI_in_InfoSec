# Application of AI for InfoSec:  Applied ML Projects

Four ML projects applying classic and deep learning techniques to security
and text-classification problems, built while working through Hack The Box's
AI Red Teamer path (Module 2: Applications of AI in InfoSec).


## Projects

| Project | Technique | Dataset |
|---|---|---|
| [Spam Classification](https://github.com/Beylessen1/Applications_of_AI_in_InfoSec/tree/main/Spam_Classification) | Naive Bayes + CountVectorizer | SMS Spam Collection |
| [Network Anomaly Detection](https://github.com/Beylessen1/Applications_of_AI_in_InfoSec/tree/main/Network_Anomaly_Detection) | Random Forest (multi-class) | NSL-KDD |
| [Malware Classification](https://github.com/Beylessen1/Applications_of_AI_in_InfoSec/tree/main/Malware_Classification) | CNN (ResNet-50, transfer learning) | Malimg |
| [Sentiment Analysis](https://github.com/Beylessen1/Applications_of_AI_in_InfoSec/tree/main/Sentiment_Analysis) | Naive Bayes + TfidfVectorizer | IMDB Reviews|

Each folder contains a notebook and a short write-up covering approach and results.

## Setup

```bash
conda create -n ai-infosec python=3.11
conda activate ai-infosec
pip install -r requirements.txt
```

Or with pip directly:

```bash
pip install -r requirements.txt
```

## Notes

The first three projects each use a meaningfully different ML approach —
text classification with Naive Bayes, tabular multi-class classification
with Random Forest, and image-based classification with a fine-tuned
ResNet-50. The sentiment analysis project is a skills-assessment exercise
using the same pipeline as the spam classifier, applied independently to
a new dataset.

## Credit

Based on Module 2 : [Applications of AI in InfoSec](https://academy.hackthebox.com/app/module/292) of the
 **AI Red Teamer Job Role Path** by **Hack The Box**,
developed in collaboration with **Google**.

<p align="center">
  <img src="./badge.png" alt="Description" />
</p>

