import spacy
from nltk import ngrams
nlp=newspacy.load("en_core_web_sn")
sentence4="""Machine Learning (ML) is the scientific study of algorithums and statistical models 
that computer system use to perform a specific task without using explict instrictions relying on patterns and
inference insted.it is seen as a subject of artifical intelligence""".

doc=nlp(sentence4)
unigrams=ngrams(doc,1)
print(list(unigrams))
bigrams=ngrams(doc,2)
print("bigrams\n",list(Bigrams))

trigrams=ngrams(doc,3)
print("trigrams\n",list(Trigrams))
