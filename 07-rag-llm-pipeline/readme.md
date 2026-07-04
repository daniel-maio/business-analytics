# Document QA Pipeline (RAG)

A Retrieval-Augmented Generation (RAG) pipeline built with **LlamaIndex** to index local unstructured documents (such as DOCX and PDFs) and query them using LLMs via **Groq API**.

This project demonstrates clean architecture for document ingestion, text splitting optimization, vector embedding generation, and semantic search retrieval.

## Examples:

- What are the payment methods?
- I would like to buy a product. Does the company offer free shipping?
- How can I contact customer service?
- Does the company offer a loyalty program? How do I sign up?
- Can I reserve a product online and pick it up in-store?

## Quickstart
```bash
pip install llama_index llama-index-llms-groq llama-index-embeddings-huggingface python-dotenv docx2txt
```

---