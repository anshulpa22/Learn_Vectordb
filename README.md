# Qdrant VectorDB Example

This project demonstrates how to use Qdrant as a vector database for storing and searching text embeddings using Python.

## Features

- Chunking large text into overlapping segments
- Generating embeddings via an external API
- Storing embeddings in Qdrant Cloud
- Semantic search using vector similarity

## Setup

1. **Install dependencies:**
   ```bash
   pip install qdrant-client numpy requests
   ```

2. **Configure Qdrant:**
   - Update your Qdrant Cloud `url` and `api_key` in the notebook.

3. **Run the notebook:**
   - Open `qdrant.ipynb` in VS Code or Jupyter and execute cells step by step.

## Usage

- The notebook creates a collection, generates embeddings for text chunks, uploads them to Qdrant, and performs a semantic search.

## Notes

- Embeddings are generated using the [euron.one](https://euron.one) API.
- Make sure your embedding size matches the collection configuration (`size=1536`).

```# Qdrant VectorDB Example

This project demonstrates how to use Qdrant as a vector database for storing and searching text embeddings using Python.

## Features

- Chunking large text into overlapping segments
- Generating embeddings via an external API
- Storing embeddings in Qdrant Cloud
- Semantic search using vector similarity

## Setup

1. **Install dependencies:**
   ```bash
   pip install qdrant-client numpy requests
   ```

2. **Configure Qdrant:**
   - Update your Qdrant Cloud `url` and `api_key` in the notebook.

3. **Run the notebook:**
   - Open `qdrant.ipynb` in VS Code or Jupyter and execute cells step by step.

## Usage

- The notebook creates a collection, generates embeddings for text chunks, uploads them to Qdrant, and performs a semantic search.

## Notes

- Embeddings are generated using the [euron.one](https://euron.one) API.
- Make sure your embedding size matches the collection configuration (`size=1536`).
# Learn_Vectordb
