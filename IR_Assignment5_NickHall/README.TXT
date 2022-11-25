Assignment 5: Using Word2Vec and Classification of Queries Using Question Tags

Description: This particular project uses Word2Vec on the Coffee Stack Exchange data to find the top-5 similar question titles to the given query and compares 
the vectors using cosine similarity. The project also uses BM25 from pyTerrier to retrieve the top-k results for a given query and determine the class of the query
using the freuqency of the question tags of the results.

Setup: Download Posts_Coffee.xml, Posts.py, post_parser_record.py. Once downloaded, the code can be ran from the top down.

Testing: Run each block from the top down and the all the cells should execute. To test the Word2Vec portion, simply run from top down. 
To run it with a different query simply change the string "query" in block 8 [8]. Function topk can then be called with the topk results as well
as the dictionary of the query topk(k, cosim_dict). The three queries: "how to make espresso", "moka pot", "coffee caffeine", and 
"can I use the same coffee grounds twice?" are used to showcase the classification of queries using question tags. In order to make additional queries, simply call 
the method getQueryClass and input the desired query followed by the desired amount of results to be retrieved. For instance, for a query "coffee caffeine" with top
10 documents being returned: getQueryClass("coffee caffeine", 10).

Usage: For Question 1, either run as is or change the string "query" in block 8 [8] to the desired query. Use function topk(k, cosim_dict) to showcase top k results.
Function table(k, cosim_dict) can also be used to showcase results. For Question 2, either run as is or use the function getQueryClass(query, k) where query is the
query to be classified and k is the number of results.
