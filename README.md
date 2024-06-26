## Pinecone Vector Database: Building a Conversational Search Agent with Pinecone

This notebook demonstrates how to create a conversational search agent using Pinecone, a vector database service. The agent leverages OpenAI for text embeddings and retrieves relevant documents from a PDF collection stored locally.

**Key functionalities:**

1. **PDF Processing:** Parses PDFs into text chunks using PyPDF2 library.
2. **Text Chunking:** Splits the extracted text into smaller chunks for efficient embedding and storage.
3. **OpenAI Embeddings:** Generates vector representations (embeddings) for each text chunk using the OpenAI API.
4. **Pinecone Integration:** Creates a Pinecone index and stores the text chunks and embeddings along with metadata like source titles.
5. **Retrieval with Text Search:** Enables searching for relevant documents based on user queries using Pinecone's similarity search functionality.
6. **Building the Agent:** Combines OpenAI for generating responses and Pinecone for document retrieval to create a conversational search experience.

**Overall Workflow:**

* PDFs are converted to text and split into chunks.
* Embeddings are generated for each chunk using OpenAI.
* The chunks, embeddings, and metadata are stored in a Pinecone index.
* A retrieval object is created to search for relevant documents based on user queries.
* The conversational agent leverages OpenAI to understand user intent and retrieves related documents from Pinecone.

## Chromadb Vector Database: Building a Conversational Search Agent with ChromaDB

This notebook showcases building a conversational search agent using ChromaDB, another vector database service. Similar to Pineconedb.ipynb, it utilizes OpenAI for text embeddings and retrieves information from a local PDF collection.

**Key functionalities:**

1. **PDF Processing:** Similar to Pineconedb.ipynb, extracts text from PDFs using PyPDF2.
2. **Text Chunking:** Splits the extracted text into manageable chunks for efficient processing.
3. **OpenAI Embeddings:** Generates embeddings for text chunks using the OpenAI API.
4. **ChromaDB Integration:** Creates a ChromaDB vector store and stores the text chunks and embeddings along with document metadata.
5. **Text Retrieval:** Enables searching for relevant documents based on user queries using ChromaDB's retrieval functionalities.
6. **Conversational Search Agent:** Combines OpenAI for response generation and ChromaDB for document retrieval to create a conversational search experience.

**Overall Workflow:**

* PDFs are converted to text and chunked for processing.
* OpenAI generates embeddings for each text chunk.
* The chunks, embeddings, and metadata are stored in a ChromaDB vector store.
* A retrieval object is created to search for relevant documents based on user queries.
* The conversational search agent interacts with the user, uses OpenAI to understand their intent, and retrieves related documents from ChromaDB.

**Similarities and Differences:**

Both notebooks build conversational search agents using similar functionalities. The key difference lies in the vector database employed: Pinecone vs. ChromaDB. The specific functionalities and syntax might differ slightly between the two services.

