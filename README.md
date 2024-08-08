# NvidiAI-Assistant-RAG-powered-Chatbot

NvidiAI Assistant is a Retrieval-Augmented Generation (RAG) powered chatbot that leverages NVIDIA AI Foundational models. This project implements a simple, standalone RAG pipeline with a Streamlit-based user interface.

## Features

- Document upload functionality to build and expand the knowledge base
- Vector database storage for efficient document retrieval
- Integration with NVIDIA AI Foundational models for embedding and language processing
- Interactive chat interface powered by a RAG pipeline

## Components

1. **Document Loader**: Allows users to upload documents to the knowledge base via a Streamlit UI.
2. **Embedding Model and LLM**: Utilizes NVIDIA AI models for document embedding and language processing.
3. **Vector Database Store**: Implements FAISS for efficient storage and retrieval of document embeddings.
4. **LLM Response Generation and Chat**: Provides an interactive chat interface that generates responses based on the uploaded documents and user queries.

## Prerequisites

- Python 3.7+
- Streamlit
- LangChain
- FAISS
- NVIDIA AI Playground API key

## Setup

1. Clone this repository
2. Install the required dependencies:
   ```
   pip install streamlit langchain faiss-cpu
   ```
3. Export your NVIDIA AI Playground API key:
   ```
   export NVIDIA_API_KEY='your_api_key_here'
   ```

## Usage

1. Run the Streamlit app:
   ```
   streamlit run app.py
   ```
2. Use the sidebar to upload documents to the knowledge base.
3. Chat with the AI Assistant using the main interface.
