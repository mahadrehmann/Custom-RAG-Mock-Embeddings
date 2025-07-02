# Local Document Q&A Chatbot with Mock Embeddings

This project implements a simple Retrieval-Augmented Generation (RAG) pipeline using custom mock embeddings instead of pre-trained ones. It enables users to load a local `.txt` document and ask questions, retrieving relevant chunks and generating simulated LLM responses.

## 🧠 Project Overview

A command-line chatbot that:
- Loads a local text file
- Splits the content into chunks
- Generates mock embeddings
- Stores chunks in a simple in-memory vector store
- Retrieves the top K relevant chunks based on cosine similarity
- Augments the query with retrieved content
- Simulates an LLM response using a mock function

This project is ideal for learning the inner workings of document retrieval, vector similarity, and chatbot logic — **without relying on external APIs or heavy libraries.**

---

## 🚀 Features

- 📂 Load any `.txt` file from your local machine
- ✂️ Custom chunking function to split large text
- 🧮 Mock embedding generator using ASCII transformations
- 🧠 Simple vector store with cosine similarity retrieval
- 🤖 Augmented prompt construction and fake LLM response generation
- 🔁 Continuous Q&A chat loop until user exits

---

## 🛠️ Tech Stack

- Python (Standard Library)
- No external libraries or frameworks

---

## 🧪 How It Works

1. **Load & Chunk Document**
   - Text is split into readable-sized chunks (default 100 chars).
2. **Generate Mock Embeddings**
   - Each character in the chunk is converted to a float using a simple formula.
3. **Vector Storage**
   - Chunks and embeddings are stored in a basic list of tuples.
4. **Query & Retrieval**
   - User's question is also embedded and cosine similarity is computed.
   - Top K relevant chunks are retrieved.
5. **Prompt Augmentation**
   - A fake LLM prompt is created using retrieved context and query.
6. **Mock Response**
   - Simulated answer is printed with reference to matched content.


