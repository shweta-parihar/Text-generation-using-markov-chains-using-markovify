# Text-generation-using-markov-chains-using-markovify

Natural Language Generation (NLG) or Text Generation is a subfield of Natural Language Processing (NLP). Its goal is to generate meaningful phrases and sentences in the form of human-written text. It has a wide range of use cases: writing long form content (eg reports, articles), product descriptions, social media posts, chatbots etc.

# Markov Chain
Markov Chain is one of the earliest algorithms used for text generation (eg, in old versions of smartphone keyboards). It is a stochastic model, meaning that it is based on random probability distribution. Markov Chain models the future state (in case of text generation, the next word) solely based on the previous state (previous word or sequence). The have ‘remain’ and ‘change’ probabilities for multi-state processes. The model is memory-less — the prediction depends only on the current state of the variable (it forgets the past states; it is independent of preceding states). On the other hand, it’s simple, fast to execute and light on memory.


# Methodology

Here, we attempt to train a model on Shakespeare's dialogues from popular plays and expect the model to generate dialogues which appear as though they might have been written by Shakespeare.  The corpus used here is the dialogues from three famous Shakespeare's plays - Hamlet, Macbeth and Julius Caeser. We have around 5000 dialogues to train the model. 
#
We use Markovify which is a python library that helps to create simple, extensible Markov chain generator. It is useful in generating random semi-plausible sentences based on an existing text. We have to specify state size - which is the number of words on which the probability of the next word depends on, I have mentioned 3 in our model. Larger state size makes our model more complex and increases the execution time. At an advanced level, such models can be used to generate poems, music notes, etc.
