# Roget's Thesaurus in the 21st Century

This project explores the structure of Roget's Thesaurus through the lens of modern Machine Learning techniques. Using word embeddings and clustering methods, we will analyze how Roget's original classification compares to data-driven groupings of word meanings. Additionally, supervised models will be used to predict word categories based on their embeddings.

## Assignment Overview
In this Jupyter notebook, you will find the following analyses:

- Extraction and preprocessing of Roget’s Thesaurus classification
- Retrieval and storage of word embeddings
- Clustering analysis to compare with Roget’s categories
- Supervised learning models for word classification by category
- Class prediction at both the class and section levels
- Evaluation of unsupervised vs. supervised methods
- Insights into agreement between data-driven clusters and thesaurus categories


## Submission Instructions

# Roget\'s Thesaurus in the 21st Century

The first known thesaurus was written in the 1st century CE by [Philo of
Byblos](https://en.wikipedia.org/wiki/Philo_of_Byblos); it was called
*Περὶ τῶν διαφόρως σημαινομένων*, loosly translated in English as *On
Synonyms*. Fast forward about two millenia and we arrive to the most
well known thesaurus, compiled by [Peter Mark
Roget](https://en.wikipedia.org/wiki/Peter_Mark_Roget), a British
physician, natural theologian, and lexicographer. [Roget\'s
Thesaurus](https://en.wikipedia.org/wiki/Roget%27s_Thesaurus) was
released on 29 April 1852, containing 15,000 words. Subsequent editions
were larger, with the latest totalling 443,000 words. In Greek the most
well known thesaurus, *Αντιλεξικόν ή Ονομαστικόν της Νεοελληνικής
Γλώσσης* was released in 1949 by [Θεολόγος
Βοσταντζόγλου](https://el.wikipedia.org/wiki/%CE%98%CE%B5%CE%BF%CE%BB%CF%8C%CE%B3%CE%BF%CF%82_%CE%92%CE%BF%CF%83%CF%84%CE%B1%CE%BD%CF%84%CE%B6%CF%8C%CE%B3%CE%BB%CE%BF%CF%85);
the latest updated edition was released in 2008 and remains an
indispensable source for writing in Greek.

Roget organised the entries of the thesaurus in a hierarchy of
categories. Your task in this assignment is to investigate how these
categories fare with the meaning of English words as captured by Machine
Learning techniques, namely, their embeddings.

Note that this is an assignment that requires initiative and creativity
from your part. There is no simple right or wrong answer. It is up to
you to find the best solution. You have three weeks to do it. Make them
count.


## Get Roget\'s Thesaurus Classification

You can find [Roget\'s Thesaurus classification online at the
Wikipedia](https://en.wiktionary.org/wiki/Appendix:Roget%27s_thesaurus_classification).
You must download the categorisation (and the words belonging in each
category), save them and store them in the way that you deem most
convenient for processing.

## Get Word Embeddings

You will embeddings for the word entries in Roget\'s Thesaurus. It is up
to you to find the embeddings; you can use any of the available models.
Older models like word2vec, GloVe, BERT, etc., may be easier to use, but
recent models like Llama 2 and Mistral have been trained on larger
corpora. OpenAI and Google offer their embeddings through APIs, but they
are not free.

You should think about how to store the embeddings you retrieve. You may
use plain files (e.g., JSON, CSV) and vanilla Python, or a vector
database.

## Clustering

With the embeddings at hand, you can check whether unsupervised Machine
Learning methods can arrive at classifications that are comparable to
the Roget\'s Thesaurus Classification. You can use any clustering method
of your choice (experiment freely). You must decide how to measure the
agreement between the clusters you find and the classes defined by
Roget\'s Thesaurus and report your results accordingly. The comparison
will be at the class level (six classes) and the section / division
level (so there must be two different clusterings, unless you can find
good results with hierarchical clustering).

## Class Prediction

Now we flip over to supervised Machine Learning methods. You must
experiment and come up with the best classification method, whose input
will be a word and its target will be its class, or its section /
devision (so there must be two different models).

## Submission Instructions

-   You must submit your assignment as a Jupyter notebook that will
    contain the full code and documentation of how you solved the
    questions, plus all accompanying material, such as embedding files,
    etc.

-   You are not required to upload your assignment; you may, if you
    wish, do your work in GitHub and submit a link to the private
    repository you will be using. If you do that, make sure to share the
    private repository with your instructor.

-   You may also include plain Python files that contain code that is
    called by your Jupyter notebook.

-   You must use [poetry](https://python-poetry.org/) for all dependency
    management. Somebody wishing to replicate your work should be able
    to do so by using the poetry file.
