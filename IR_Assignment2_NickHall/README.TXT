Assignment 2 Inverted Index Retrieval System

Description: This particular project gathers question and answer data of thousands of posts on the Coffee Stack Exchange website
and builds an inverted index based on the tokens in the question and answer data to be used for retrieval.

Setup: Download Posts_Coffee.xml, Posts.py, post_parser_record.py, and skijump.JPG and have them ready to import.
Once imported, the code can be ran from the top down.

Testing: Run each block from the top down and the all the cells should execute. The three queries: "espresso", "turkish coffee", and "persian coffee"
are the only ones displayed, however, a new query search can be made by simply calling freq_search(query).

Usage: freq_search(query) can be used to identify question/answer documents relevant to the query, based on an inverted index sorted by the count
that each search term appears in the document.