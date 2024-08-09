# NHS Care Bot - README

## Overview

This repository contains the code for a healthcare chatbot named **NHS Care Bot**, developed specifically for UK NHS Hospitals. The bot is designed to provide users with information and support based on the official NHS data, with a strong focus on patient safety and accurate guidance. The chatbot uses state-of-the-art language models and vector databases to process and retrieve information.

## Features

1. **Document Loader**:
   - Allows users to upload documents to a knowledge base.
   - Automatically organizes and stores these documents for future processing.

2. **Embedding Model and Language Model**:
   - Uses NVIDIA's AI models for text embedding and natural language understanding.
   - Generates responses based on the context provided by the user and documents in the knowledge base.

3. **Vector Database Store**:
   - Efficiently stores and retrieves information using a vector store (FAISS).
   - Can utilize an existing vector store or create a new one from uploaded documents.

4. **LLM Response Generation and Chat**:
   - Provides a user interface for interacting with the chatbot.
   - Generates context-aware responses to user queries based on the knowledge base.

## How to Use

### 1. Set Up

- Ensure you have the required dependencies installed. You can install them using the following:
  ```bash
  pip install streamlit langchain_nvidia_ai_endpoints langchain_core
  ```

- Set your NVIDIA API key as an environment variable:
  ```bash
  export NVIDIA_API_KEY='your_api_key_here'
  ```

### 2. Run the Application

- Start the Streamlit application:
  ```bash
  streamlit run app.py
  ```

- The application will launch in your browser, where you can interact with the chatbot.

### 3. Uploading Documents

- Navigate to the sidebar and upload documents that will form the basis of the knowledge base.
- Uploaded files will be stored in the `uploaded_docs` directory.

### 4. Using the Vector Store

- You can choose to use an existing vector store or create a new one based on the uploaded documents.
- If you choose to create a new store, the documents will be split into chunks and embedded for efficient retrieval.

### 5. Chat Interface

- Type your message in the chat input field.
- The bot will respond based on the context derived from the uploaded documents.

## Important Notes

- **Disclaimer**: The chatbot is an AI assistant and should not be considered a substitute for professional medical advice. It provides information based on the context it has been given and the official NHS guidelines. Users are encouraged to consult healthcare professionals for personalized advice.

## File Structure

- `app.py`: The main application file.
- `uploaded_docs/`: Directory where uploaded documents are stored.
- `vectorstore.pkl`: Serialized vector store file for quick retrieval.

## Dependencies

- `Streamlit`: Used for building the web interface.
- `Langchain`: Framework for working with language models and vector databases.
- `FAISS`: Library for efficient similarity search and clustering of dense vectors.
- `NVIDIA AI Models`: State-of-the-art models for text embedding and response generation.

## License

This project is licensed under the MIT License. Please see the `LICENSE` file for more details.

---

For any issues or contributions, please feel free to submit a pull request or open an issue on the repository.
