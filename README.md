# Markov-chain-for-text-generation
Aim:- Our motivation behind this project is to make a probabilistic model that can predict the text based on previous state of outputs.

Data Prepration Part:-

  Training Data:-
    It's just a usual corpus of data.
  Test Data:-
    Data train on runtime only, so no test data.

Model Planning:-
  We'll use markov model, the best part about the markov model is that the future state depends only on current state, in witch there are   two states one is transmission probalility and other is emission probibility. Here we select the k end letters to predict the next         letter and after generating that letter we took again previous k letter and again next letter, this is iterative method and goes on.
  
Model Building:-
  Here we iterate from starting till the end (range k to n), iterating over a batch of k letters and storing them in a dictonary as a key
  along with the next the letter and it's probability according it's occurance.
  
Enhacing and Evaluating the Model:- As dictonary is being prepared we will iterate over the test sentance section and will select the last k letters so as to predict the next letter.
