# Topic-Modeling-on-News-Articles

Latent Dirichlet Allocation

This notebook is a part of my learning journey which I've been documenting from Udacity's Natural Language Processing Nanodegree program, which helped me a lot to learn and excel advanced data science stuff such as PySpark. Thank you so much Udacity for providing such quality content.

LDA is used to classify text in a document to a particular topic. It builds a topic per document model and words per topic model, modeled as Dirichlet distributions.

Each document is modeled as a multinomial distribution of topics and each topic is modeled as a multinomial distribution of words.

LDA assumes that the every chunk of text we feed into it will contain words that are somehow related. Therefore choosing the right corpus of data is crucial.

It also assumes documents are produced from a mixture of topics. Those topics then generate words based on their probability distribution.

Data Preprocessing

We will perform the following steps:


Tokenization: Split the text into sentences and the sentences into words. Lowercase the words and remove punctuation.

Words that have fewer than 3 characters are removed.

All stopwords are removed.

Words are lemmatized - words in third person are changed to first person and verbs in past and future tenses are changed into present.

Words are stemmed - words are reduced to their root form.

TF-IDF stands for "Term Frequency, Inverse Document Frequency".

It is a way to score the importance of words (or "terms") in a document based on how frequently they appear across multiple documents.

If a word appears frequently in a document, it's important. Give the word a high score. But if a word appears in many documents, it's not a unique identifier. Give the word a low score.
