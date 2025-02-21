README.md

# Proj1
This repository demonstrates the use of DeepSeek-R1 Document RAG with Streamlit

## Table of contents
1.[Overview](#overview)
2.[Prerequisites](#prerequisite)
3.[setup and installation](#setup_and_installation)
4.[Dataset details](#dataset_details)
5.[implementation steps](#implementation_steps)

## overview
This project demonstrates a robust RAG (Retrieve, Augment, Generate) system designed for question answering on PDF documents. It combines the capabilities of the DeepSeek-R1 large language model with the efficiency of ChromaDB for information retrieval. The system processes uploaded PDF documents, retrieves relevant information based on user queries, and generates comprehensive answers.

## prerequisites
Python 3.8 or higher
Access to DeepSeek-R1 large language model
Access to ChromaDB
Access to Hugging Face Embeddings
Streamlit for the user interface
UnstructuredPDFLoader for document processing
RecursiveCharacterTextSplitter for text segmentation

## setup and installation
**Install Python:** Ensure you have Python 3.8 or higher installed.
**Install Dependencies:** Install the required Python packages using:
**Set Up ChromaDB:** Follow the instructions to set up ChromaDB.
**Set Up DeepSeek-R1**: Ensure you have access to the DeepSeek-R1 model.
**Set Up Streamlit:** Install Streamlit using:

## Dataset details
**Document Processing:** Uploaded PDFs are processed using the UnstructuredPDFLoader to extract textual content. The RecursiveCharacterTextSplitter segments this text into manageable chunks.
**Embedding Creation:** Semantic embeddings are generated for each text chunk using Hugging Face Embeddings, capturing the contextual meaning of the information.
**Vector Storage:** ChromaDB serves as the vector database, storing the embeddings and enabling rapid similarity searches.

## implementation steps
# Document Processing:
Use UnstructuredPDFLoader to extract text from uploaded PDFs.
Segment the extracted text into manageable chunks using RecursiveCharacterTextSplitter.
# Embedding Creation:
Generate semantic embeddings for each text chunk using Hugging Face Embeddings.
# Vector Storage:
Store the embeddings in ChromaDB for efficient similarity searches.
# Query Processing and Retrieval:
Embed user queries using the same embedding model.
Query ChromaDB to retrieve the most relevant document chunks based on the user query.
# Answer Synthesis:
Input the retrieved chunks and the user query to the DeepSeek-R1 model.
Generate a comprehensive answer using the model.
# User Interaction:
Implement a Streamlit-based interface for seamless document upload and query submission.
Enhance user experience by providing a user-friendly interface for interacting with the system.









# DeepSeek-R1 Document RAG with Streamlit

This project demonstrates a robust RAG system designed for question answering on PDF documents.  It combines the capabilities of the DeepSeek-R1 large language model with the efficiency of ChromaDB for information retrieval.  The workflow comprises the following steps:
**1. Document Processing:** Uploaded PDFs are processed using the UnstructuredPDFLoader to extract textual content. The RecursiveCharacterTextSplitter segments this text into manageable chunks.
**2. Embedding Creation:** Semantic embeddings are generated for each text chunk using Hugging Face Embeddings, capturing the contextual meaning of the information.
**3. Vector Storage:** ChromaDB serves as the vector database, storing the embeddings and enabling rapid similarity searches.
**4. Query Processing and Retrieval:** User queries are embedded using the same model, and ChromaDB is queried to retrieve the most relevant document chunks.
**5. Answer Synthesis:** The retrieved chunks and the user query are input to the DeepSeek-R1 model, which generates a comprehensive answer.
**6. User Interaction:** A Streamlit-based interface provides seamless document upload and query submission, enhancing user experience.
