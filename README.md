# DeepSeek-R1 Document RAG with Streamlit

This project demonstrates a robust RAG system designed for question answering on PDF documents.  It combines the capabilities of the DeepSeek-R1 large language model with the efficiency of ChromaDB for information retrieval.  The workflow comprises the following steps:
**1. Document Processing:** Uploaded PDFs are processed using the UnstructuredPDFLoader to extract textual content. The RecursiveCharacterTextSplitter segments this text into manageable chunks.
**2. Embedding Creation:** Semantic embeddings are generated for each text chunk using Hugging Face Embeddings, capturing the contextual meaning of the information.
**3. Vector Storage:** ChromaDB serves as the vector database, storing the embeddings and enabling rapid similarity searches.
**4. Query Processing and Retrieval:** User queries are embedded using the same model, and ChromaDB is queried to retrieve the most relevant document chunks.
**5. Answer Synthesis:** The retrieved chunks and the user query are input to the DeepSeek-R1 model, which generates a comprehensive answer.
**6. User Interaction:** A Streamlit-based interface provides seamless document upload and query submission, enhancing user experience.
