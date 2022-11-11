Project Part 2

Description: This particular project gathers question and answer data of hundreds of thousands of posts on the Science Fiction and Fantasy stack exchange website
and uses a variety of different models to retrieve the results of 20 real queries that I chose from the stack exchange. The project also investigates and analyzes
the results of the different models. The code implements seven models of retrieval: TF-IDF, BM25, PL2, Reranked BM25 using TF-IDF, Fusion of TF-IDF and BM25 using
CombMNZ, Weighted Combination of BM25 and TF-IDF, and Query Expansion on BM25 using RM3. This project uses PyTerrier and Ranx for models and evaluation.

Setup: Download SPosts.xml (from the stack exchange website), Posts.py, qrel.tsv and post_parser_record.py and have them ready to import.
Once imported, the code can be ran from the top down.

Testing: Run each block from the top down and all the cells should execute as intended. If the intention is to diverge from my model, this can be done after 
the index has been created. New models can be added simply by reading PyTerrier documentation and appending these models to the existing code. To run your own 
queries through the desired models, simply change the values in the "queries" dataframe with your query. 


Usage: After the index has been created, the user has the freedom to see the retrieval results for any model that PyTerrier or Ranx includes. Queries to
input into these models can be altered in the queries dataframe as long as it follows the "qid" "query" format. .transform(queries) can be called after using PyTerriers'
batch retrieve method in order to get the query results.
