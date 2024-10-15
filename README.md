# Retrieval-Augmented-Generation-RAG-Model
This repository contains an implementation of a Retrieval-Augmented Generation (RAG) pipeline for answering questions based on a corpus of documents. It leverages a pre-trained RAG model from Facebook AI (facebook/rag-token-nq) for document retrieval and text generation, and answer extraction from retrieved documents.

Features
Document Retrieval: Finds top k most relevant documents from a preprocessed corpus based on a query.
Fact Extraction: Extracts key facts from the top retrieved documents using deepset/roberta-base-squad2.
Answer Generation: Generates an answer to the user's query by synthesizing information from the most relevant document.
Model Architecture
Query Embedding: The query is encoded into an embedding using facebook/rag-token-nq.
Document Retrieval: Top k documents are retrieved based on cosine similarity between the query embedding and document embeddings.
Fact Extraction: Key facts are extracted from the top k documents using deepset/roberta-base-squad2.
Answer Generation: The most relevant document is used to generate an answer to the query.
