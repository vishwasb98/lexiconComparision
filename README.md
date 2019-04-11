# lexiconComparision
We have implemented AFINN, SentiWordNet and VADER Lexicons. We further calculate their metrics from the sklearn library to find out which of these work with the best Accuracy, Precision, Recall and F1 score.
The implementation is basically divided into 3 major pyhton files, with each having their own
functionalities:
1. text_normalizer.py
text_normalizer.py is the python file which helps us in implementing the preprocessing on
the texts to make them understandable by the lexicons. This has all the functionalities mentioned in
previous section named Text Pre-Processing and Normalization.
2. unsupervised_sentiment_analysis.py
unsupervised_sentiment_analysis.py is the implementation af all the three lexicons, AFINN ,
SentiWordNet and VADER with the sample reviews being analysed and sentiments being printed.
At the end of the file, a comparition is shown.
3. model_evaluation_utils.py
model_evaluation_utils.py is the python file which helps in calculation various metrics to
assess the quality, rigidity and the varience between the predicted outcomes and the ground truth.
This will help us in comparing between various lexicons.
Other python files such as contrations.py are also present which play trivial roles in text
normalization.

Lexicons
1. AFINN Lexicon
The AFINN lexicon is perhaps one of the simplest and most popular lexicons that
can be used extensively for sentiment analysis. Developed and curated by Finn Årup Nielsen, you
can find more details on this lexicon in the paper by Finn Årup Nielsen, “A new ANEW: evaluation
of a word list for sentiment analysis in microblogs”, proceedings of the ESWC2011 Workshop. The
current version of the lexicon is AFINN-en-165. txt and it contains over 3,300+ words with a
polarity score associated with each word.
2. SentiWordNet Lexicon
The WordNet corpus is definitely one of the most popular corpora for the English
language used extensively in natural language processing and semantic analysis. WordNet gave us
the concept of synsets or synonym sets. The SentiWordNet lexicon is based on WordNet synsets and
can be used for sentiment analysis and opinion mining. The SentiWordNet lexicon typically assigns
three sentiment scores for each WordNet synset.These include a positive polarity score, a negative
polarity score and an objectivity score.
3. VADER Lexicon
The VADER lexicon, developed by C.J. Hutto, is a lexicon that is based on a rule-
based sentiment analysis framework, specifically tuned to analyze sentiments in social media.
VADER stands for Valence Aware Dictionary and Sentiment Reasoner. Details about this
framework can be read in the original paper by Hutto, C.J. & Gilbert, E.E. (2014) titled “VADER: A
Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text”, proceedings of the
Eighth International Conference on Weblogs and Social Media (ICWSM-14). You can use the
library based on nltk's interface under the nltk.sentiment.vader module.


The above result shows that for a given dataset, SentiWordNet is more accurate than
VADER and AFINN. It has more Recall and F1 Score too.
But as for Precision, AFINN and VADER Lexicon work better than SentiWordNet.
