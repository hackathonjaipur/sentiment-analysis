# sentiment-analysis
#It is a model in transformer in which we can analysis sentiments in a sentence , and rate them , we can also analysis sentences of different languages.
pip install transformers
from transformers import pipeline
classifiers = pipeline('sentiment-analysis',model ="nlptown/bert-base-multilingual-uncased-sentiment")
# it is a french sentence "the food is delicious" here we can see that it is a positive sentence .
classifiers ('la nourriture est délicieuse')
# here we are using  a english sentence .
classifiers("you are very bad ")
