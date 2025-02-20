# DeepSeek-R1 Document RAG with Streamlit

This project demonstrates a Retrieval Augmented Generation (RAG) application using DeepSeek-R1 and Streamlit. It allows users to upload a PDF document, ask questions about its content, and receive answers powered by the DeepSeek-R1 model.  The project uses ChromaDB for efficient storage and retrieval of document chunks.

## Project Overview

This project showcases a practical application of the RAG paradigm, combining document processing, vector embeddings, and large language models for intelligent question answering.  The architecture incorporates:

Document Loading and Chunking: Utilizes UnstructuredPDFLoader and RecursiveCharacterTextSplitter for efficient document parsing and text segmentation.
Semantic Embeddings: Employs Hugging Face Embeddings to generate vector representations of text, capturing semantic relationships.
Vector Database Management: Leverages ChromaDB for persistent storage and efficient retrieval of document embeddings.
Large Language Model Integration: Integrates the DeepSeek-R1 model for context-aware answer generation.
User Interface Development: Implements a user-friendly interface using Streamlit, facilitating document upload and query input.
