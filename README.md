# Deciphering-Code

The dataset we have consists of 10,000 encrypted phrases and the plaintext version of each encrypted phrase.The model we will use here is a character-level RNN since the cipher seems to work on the characer level.
A character-level RNN will take as input an integer referring to a specific character and output another integer. To be able to get our model to work, we'll need to preprocess our dataset in the following steps:

1-Isolating each character as an array element (instead of an entire phrase, or word being the element of the array)
2-Tokenizing the characters so we can turn them from letters to integers and vice-versa
3-Padding the strings so that all the inputs and outputs can fit in matrix form
