Assignment 3: Implementation of TF-IDF, VSM, and BM25

Description: This particular project gathers and stores the question and answer data of thousands of posts on the Coffee Stack Exchange website
which can be used by the three implemented retrieval models: TF-IDF, VSM, and BM25. 

Setup: Download Posts_Coffee.xml, Posts.py, post_parser_record.py. Once downloaded, the code can be ran from the top down.

Testing: Run each block from the top down and the all the cells should execute. The four queries: "espresso", "turkish coffee", 
"making a decaffeinated coffee", and "can I use the same coffee grounds twice?" are used to showcase the three retrieval models.
In order to make additional queries, simply call the method top_k and input the desired retrieval model with the query as an input as well as the desired
amount of results to be retrieved. 
For instance, for a query "espresso" using the BM25 model with top 10 documents being returned: 
top_k(bm25("can I use the same coffee grounds twice?"), 10)

Usage: Each of the three models will display the top ranked documents that best match the query according to the model. To get a full list of the top 
ranked results call the method for the desired retrieval model with the query as an argument. To get the top k results, call 
the method top_k and input the desired retrieval model with the query as an input as well as the desired k of results to be retrieved. 
