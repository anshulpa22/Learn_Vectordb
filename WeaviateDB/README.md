# Weaviate Vector Database Example

This project demonstrates how to use Weaviate as a vector database to store and query text embeddings. It includes an example of uploading text data with embeddings and performing semantic search.

## Features

- Converts text data into embeddings using an external API.
- Uploads text data and embeddings to a Weaviate cluster.
- Performs semantic search queries on the stored data.

## Setup

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Configure Weaviate:**
   - Replace the `url` and `api_key` in the script with your Weaviate instance details.

3. **Run the script:**
   - Open the notebook `weaviatedb.ipynb` and execute the cells step by step.

## Usage

### Upload Data
- The script processes a dataset of text, generates embeddings, and uploads them to the Weaviate cluster.
- Each record includes:
  - A unique ID
  - The embedding vector
  - The associated text

### Query Data
- Perform semantic search using a query embedding:
  ```python
  response = client.query.get(
      "Document",                # Class name
      ["text"]                   # Properties to return
  ).with_near_vector({
      "vector": query_embedding, # Query embedding
      "certainty": 0.7           # Optional: confidence threshold
  }).with_limit(3).do()

  # Print results
  for result in response["data"]["Get"]["Document"]:
      print(result["text"])
  ```

## Notes

- Ensure your Weaviate class schema matches the uploaded data structure.
- The embedding model used is `text-embedding-3-small` from an external API.

## Requirements

See `requirements.txt` for the list of dependencies.

---
Happy Learning!