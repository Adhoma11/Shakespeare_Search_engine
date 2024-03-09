# Shakespeare_Search_engine
# **Project Summary: Building a Shakespeare Search Engine**

In this project, we set out to create a search engine for exploring the works of William Shakespeare. The dataset consisted of 44 Shakespearean books, and our goal was to construct a tool that allows users to search for specific words or combinations of words within these literary works.

**Key Steps:**

**Indexing the Books:**

We began by creating a binary search tree, a data structure that helps organize and retrieve words from the books efficiently. Each node in the tree represented a unique word, and the associated documents were stored in a list.

**Text Normalization:**

To enhance search accuracy, we applied normalization techniques, including case folding (making all text lowercase), removing stop words (common words like "the," "and," etc.), lemmatization (reducing words to their base form), and stemming (reducing words to their root).

**Query Parsing and Execution:**

Users can input queries, combining words with operators like OR and AND. We implemented a query parser to interpret these queries, considering parentheses and applying the specified operators. The search engine then retrieved documents matching the query criteria.

**Handling Missing Words:**

In cases where a word wasn't found in the tree, we implemented a mechanism to suggest the closest matching word using the Levenshtein algorithm (edit distance).

**Query Rules and Result Display:**

The search engine supports both AND and OR operations in queries, allowing users to refine their searches. The results, along with the elapsed time for each query, are presented to the user.
