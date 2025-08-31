# Pinecone VectorDB Example

This directory contains an example of using Pinecone, a managed vector database, for storing and querying text embeddings in Python.

## Features

- Converts research text into embeddings using an external API
- Stores embeddings and metadata in Pinecone
- Performs semantic search queries on the stored data

## Setup

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Configure Pinecone:**
   - Set your Pinecone API key in the script or as an environment variable.

3. **Run the notebook:**
   - Open `pinecone.ipynb` and execute the cells step by step.

## Usage

- The notebook demonstrates how to:
  - Prepare and clean text data
  - Generate embeddings for each text segment
  - Upsert vectors into Pinecone
  - Query Pinecone for semantic search

## Notes

- Embeddings are generated using the [euron.one](https://euron.one) API.
- Make sure your embedding size matches the Pinecone index configuration.
