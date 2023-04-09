# Language-Models


### Comparison of N-gram, Good Turing and Kneser-Ney language models to Recurrent Neural Networks by evaluating the perplexity of the language models

#### - N-gram, Good Turing and Kneser-Ney Language Models are statistical language modeling techniques used for prediction of word sequences using probability

#### - RNNs are based on deep learning that can learn model sequential data and language. RNN’s were developed for language modeling.

#### - N-gram Language Model: N-gram models are based on the idea of estimating the probability of a word based on the context of its preceding N-1 words, where N is a positive integer. N-gram models are simple and widely used in NLP due to their computational efficiency. They rely on the assumption that the probability of a word depends only on the N-1 words that precede it, and they estimate the conditional probabilities using frequency counts from a training corpus.

#### Learn More: Language Models: N-GramTowards Data Sciencehttps://towardsdatascience.com › introduction-to-langu...

#### -Good Turing Language Model: The Good-Turing smoothing technique is a statistical method used to estimate the probabilities of rare or unseen events in N-gram models. It is based on the idea of using the observed frequency of events that occur once (i.e., "singletons") to estimate the probabilities of events that have not been observed in the training data. Good-Turing smoothing adjusts the frequency counts of events based on the expected frequency of events that occur only once, resulting in more accurate probability estimates for rare events.

#### Learn More: An Empirical Study of Good-Turing Smoothing for ...Scientific Research Publishinghttps://www.scirp.org › journal › PaperDownload

#### -Kneser-Ney Language Model: The Kneser-Ney smoothing technique is a more advanced method for estimating the probabilities of N-grams, specifically for handling the issue of data sparsity in N-gram models. Kneser-Ney smoothing uses the concept of "discounting" to redistribute the probability mass from higher frequency N-grams to lower frequency ones, and it also uses "backoff" to combine lower-order N-gram probabilities when higher-order N-grams are not observed.

#### Learn More: A simple numerical example for Kneser-Ney Smoothing ...Mediumhttps://medium.com › a-simple-numerical-example-for...

#### -Recurrent Neural Networks: RNNs use recurrent connections to maintain hidden state that allows them to capture long-range dependencies in sequences. RNNs are more complex and computationally expensive compared to N-gram models, but they can learn from large amounts of data and capture complex patterns in language data.

#### Learn More: Recurrent Neural Networks (RNNs)Towards Data Sciencehttps://towardsdatascience.com › recurrent-neural-net...


### Concept of Perplexity

#### - Perplexity is an intrinsic way of evaluating a language model by quantifying how well it can predict a given sequence of words

#### Learn More: Perplexity in Language Models. Evaluating ...Towards Data Sciencehttps://towardsdatascience.com › perplexity-in-langua...

### Details About the RNN Language Model:

#### - Input words are converted into word embeddings and then fed to the RNN Model
#### - Vocab Size is the number of unique words in the text corpus
#### - There are 128 hidden layers
#### - Sequence to Sequence loss is used because input and output sequences have varying lengths
#### - ADAM is used for the minimizing the Sequence to Sequence loss, basically optimizing the RNN model
#### - The RNN model is trained on batches of word embeddings and the batch size is 256
#### - The final train loss obtained is 1.3506 and the valid loss obtained is 0.8225 after 30 iterations

### Only the RNN model’s architecture is built using Tensorflow, all the other parts of the program are written from scratch with the aim of understanding how the language models work.





