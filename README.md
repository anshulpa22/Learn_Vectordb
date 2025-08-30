# Learn_Vectordb

This repository contains learning material and practical examples for working with vector databases in Python, including Qdrant and ChromaDB.

## Contents

- **Qdrant Example:** Store and search text embeddings using Qdrant.
- **ChromaDB Example:** Build a local vector database with ChromaDB for semantic search.
- **Python Scripts & Notebooks:** Step-by-step guides and code for vector database operations.

## ChromaDB Example

The ChromaDB notebook demonstrates:
- Installing ChromaDB
- Creating a collection
- Generating embeddings for text data
- Adding documents and embeddings to the collection
- Performing semantic queries on the stored data

## Setup

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

- Run the notebooks or Python scripts in this repository to explore vector database features.
- Example for ChromaDB:
  ```python
  import chromadb
  client = chromadb.Client()
  # See chromadb.ipynb for full workflow
  ```

## Requirements

See `requirements.txt` for all necessary Python packages.

---
Happy Learning!