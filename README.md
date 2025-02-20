README.md

## Proj - 1
This repository demonstrates the use of DeepSeek-R1 Document RAG with Streamlit

## Table of contents
1.[Overview](#overview)<br>
2.[Prerequisites](#prerequisite)<br>
3.[setup and installation](#setup_and_installation)<br>
4.[Dataset details](#dataset_details)<br>
5.[implementation steps](#implementation_steps)<br>

## overview
This project demonstrates a robust RAG (Retrieve, Augment, Generate) system designed for question answering on PDF documents. It combines the capabilities of the DeepSeek-R1 large language model with the efficiency of ChromaDB for information retrieval. The system processes uploaded PDF documents, retrieves relevant information based on user queries, and generates comprehensive answers.

## prerequisites

- Python 3.8 or higher
- Access to DeepSeek-R1 large language model
- Access to ChromaDB
- Access to Hugging Face Embeddings
- Streamlit for the user interface

## Setup and installation
**1. Install Python:** 
Ensure you have Python 3.8 or higher installed.<br>
**2. Install Dependencies:**
Install the required libraries using requirement.txt.<br>
**3. Set Up DeepSeek-R1:** 
Ensure you have access to the DeepSeek-R1 model.<br>

## implementation steps
**1. Document Processing:**
Use UnstructuredPDFLoader to extract text from uploaded PDFs.
Segment the extracted text into manageable chunks using RecursiveCharacterTextSplitter.<br>
**2. Embedding Creation:**
Generate semantic embeddings for each text chunk using Hugging Face Embeddings.<br>
**3. Vector Storage:**
Store the embeddings in ChromaDB for efficient similarity searches.<br>
**4. Query Processing and Retrieval:**
Embed user queries using the same embedding model.
Query ChromaDB to retrieve the most relevant document chunks based on the user query.<br>
**5. Answer Synthesis:**
Input the retrieved chunks and the user query to the DeepSeek-R1 model.
Generate a comprehensive answer using the model.<br>
**6. User Interaction:**
Implement a Streamlit-based interface for seamless document upload and query submission.
Enhance user experience by providing a user-friendly interface for interacting with the system.

