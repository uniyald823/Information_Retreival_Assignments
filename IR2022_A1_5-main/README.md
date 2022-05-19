# IR2022_A1_5
CSE 508 Information Retrieval Assignment I
[IR Assignment 1 Readme.pdf](https://github.com/shashankrustagiiiitdelhi/IR2022_A1_5/files/8160768/IR.Assignment.1.Readme.pdf)

Question 1. 
(a) Carry out the suitable preprocessing steps on the given dataset.
(b) Implement the unigram inverted index data structure.
(c) Provide support for the following queries-
(i) (1 point) x OR y
(ii) (1 point) x AND y
(iii) (2 points) x AND NOT y
(iv) (2 points) x OR NOT y


Note-
• Try to write generalized code where the number of words in the query can be variable. The queries
can be of more than 2 words of the form: ”x OP1 y OP2 z” where OP1, OP2 = AND, OR, NOT.
• Perform preprocessing on the input query as well.
• The number of operations specified for a query would be under the assumption that the suitable
preprocessing steps have been applied.
Input format:
The first line contains the number of queries, N.
The next 2N lines would represent the queries.
Each query would consist of two lines:
(a) line 1: Input sentence
(b) line 2: Input operation sequence

Some example queries-
1. Input query: lion stood thoughtfully for a moment

Input operation sequence: [ OR, OR , OR ]
Expected query after preprocessing: lion OR stood OR thoughtfully OR moment
Output- Number of documents matched: 270
No. of comparisons required: 671
2. Input query: telephone,paved, roads
Input operation sequence: [ OR NOT, AND NOT ]
Expected query after preprocessing: telephone OR NOT paved AND NOT roads
Output- Number of documents matched: 466
No. of comparisons required: 739


Question 2
Use the same dataset given in the previous question.
(a) Carry out the following preprocessing steps on the given dataset
(i) Convert the text to lower case
(ii) Perform word tokenization
(iii) Remove stopwords from tokens
(iv) Remove punctuation marks from tokens
(v) Remove blank space tokens
(b) Implement the positional index data structure
(c)  Provide support for the searching of phrase queries. You may assume query length to be
less than or equal to 5.
