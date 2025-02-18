# RAG Chatbot App

## Introduction
The **RAG Chatbot App** is a Python-based application designed to enable users to interact with multiple PDF documents using natural language. By leveraging a **Retrieval-Augmented Generation (RAG)** approach, the app provides precise answers based on the content of the loaded PDFs. It ensures that responses are strictly relevant to the provided documents, enhancing accuracy and reliability.

## How It Works
The application follows a structured pipeline to process user queries effectively:

1. **PDF Loading**: The app reads and extracts text from multiple PDF documents.
2. **Text Chunking**: The extracted text is divided into manageable chunks for efficient processing.
3. **Vector Embeddings**: A language model generates vector representations (embeddings) of the text chunks.
4. **Similarity Matching**: When a user asks a question, the app identifies the most semantically relevant chunks.
5. **Response Generation**: The most relevant chunks are processed by the language model to generate an accurate response.

## Installation & Dependencies
To install and set up the RAG Chatbot App, follow these steps:

### Prerequisites
- Python 3.8 or later
- OpenAI API Key
- Required Python packages (listed in `requirements.txt`)

### Installation Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/NikitaPawar15/rag-chatbot.git
   cd rag-chatbot
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up the OpenAI API key in a `.env` file:
   ```bash
   echo "OPENAI_API_KEY=your_secret_api_key" > .env
   ```

## Usage
To run the application:

1. Ensure all dependencies are installed and the OpenAI API key is set up.
2. Start the application using Streamlit:
   ```bash
   streamlit run main.py
   ```
3. The app will open in your default web browser.
4. Upload multiple PDF documents via the interface.
5. Ask questions in natural language, and the chatbot will provide answers based on the loaded PDFs.

## Features
- **Multi-PDF Support**: Load multiple PDF documents simultaneously.
- **AI-Powered Responses**: Uses advanced natural language processing for accurate answers.
- **User-Friendly Interface**: A simple, intuitive UI powered by Streamlit.
