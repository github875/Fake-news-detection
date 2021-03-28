# Fake-news-detection
# Fake News Classifier

## Investigating Fake News Detection with Scikit-Learn

Detecting so-called “fake news” is no easy task. First, we need to deﬁne what fake news is – given it has now become a political statement. If you can ﬁnd or agree upon a deﬁnition, then you must collect and properly label real and fake news (hopefully on similar topics to best show clear distinctions). Once collected, you must then ﬁnd useful features to determine fake from real news.

## Building Vectorizer Classiﬁers

After we have both training and testing data, we can build your classiﬁers. Classifiers are used to get a good idea if the words and tokens in the articles had a signiﬁcant impact on whether the news was fake or real. Two such vectorizer classifiers used in the project are:-
1. CountVectorizer  
2. TfidfVectorizer
The CountVectorizer uses bag-of-words model to give the word count vectors whereas the TfidfVectorizer uses TF-IDF matrix to remove words that occur more frequently throughout the articles and are not much useful like are, that, is etc.

## Applying models and comparing them

The following models were used to compare TF-IDF with bag-of-words:-
1. MultinomialNB
   On using MultinomialNB, it was found that count vectorized training set count_train visibly outperformed the TF-IDF vectors.
2. Passive Agressive classiﬁer
   On using Passive Agressive classiﬁer, it was found that TF-IDF performed better than the CountVectorizer using bag-of-words concept.

## HashingVectorizer 

Another vectorizer used sometimes for text classiﬁcation is a HashingVectorizer. HashingVectorizers require less memory and are faster (because they are sparse and use hashes rather than tokens) but are more difﬁcult to introspect.
