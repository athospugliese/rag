# Document Retrieval System (RAG) with Elasticsearch and Local Llama

This project demonstrates how to create a Retrieval-Augmented Generation (RAG) system using Elasticsearch for semantic search and a local Llama model to answer queries based on the retrieved documents.

---

## Technologies Used

- **Elasticsearch**: For indexing and retrieving documents.
- **LangChain**: For integrating documents, embeddings, and the Llama model.
- **Local Llama**: Language model for natural language processing and response generation.
- **Nomic Embeddings**: To generate semantic representations of text.

---

## System Workflow

1. **Document Loading**:
   - Use `WebBaseLoader` or load local documents to build the knowledge base.

2. **Text Splitting**:
   - Split documents into smaller chunks using `RecursiveCharacterTextSplitter` to optimize retrieval.

3. **Embedding Generation**:
   - Generate semantic vectors for text chunks using the `nomic-embed-text-v1.5` model.

4. **Indexing in Elasticsearch**:
   - Store embeddings and texts in Elasticsearch to enable fast semantic search.

5. **Retrieval and Generation**:
   - Given a query, retrieve relevant documents from Elasticsearch and pass them to the local Llama model for a context-based response.

---
