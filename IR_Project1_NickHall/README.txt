Project 1

Description: This particular project gathers question and answer data of hundreds of thousands of posts on the Science Fiction and fantasy stack exchange website
and builds an inverted index based on the tokens in the question and answer data to be used for retrieval. The project also investigates and analyzes the stack exchange. 
The code implements two systems of retrieval: a boolean retrieval system and an inverted index retrieval which retrieves based on the frequency that each query appears 
in each posting. 

Setup: Download SPosts.xml (from the stack exchange website), Posts.py, and post_parser_record.py and have them ready to import.
Once imported, the code can be ran from the top down.

Testing: Run each block from the top down and the all the cells should execute. For the boolean retrieval system, additional queries can be retrieved by using 
boolean_search_or(query) or boolean_search_and(query). For the inverted index retrieval system, additonal queries can be retrieved by using freq_search(query).
To display the results of these functions, use the method top_k(r, k) where r is the result of one of the other function calls and k is the amount of results 
you want returned.

Usage: boolean_search_or(query) can be used to identify question/answer documents relevant to the query, based on a boolean 'or' between each document containing 
a search term. boolean_search_and(query) can be used to identify question/answer documents relevant to the query, based on a boolean 'and' between each document 
containing a search term. freq_search(query) can be used to identify question/answer documents relevant to the query, based on an inverted index sorted by the count
that each search term appears in the document.
