# Mini RAG Pipeline

A small retrieval-augmented generation (RAG) pipeline in Python.

## How it works
document -> chunk -> TF-IDF vectors -> question vector -> cosine similarity -> top matches -> prompt

## Features
- Chunks a document into sentences
- Ranks chunks with TF-IDF and cosine similarity
- Removes stop words to avoid false matches on common words
- Similarity threshold: returns "I don't know" when nothing is relevant
- Builds a context-grounded prompt for an LLM

## Limitations and next steps
- TF-IDF matches exact words, not meaning
- Next: sentence embeddings, a vector database (Chroma) and an LLM API call

## Tech
Python, Scikit-Learn
