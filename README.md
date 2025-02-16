# 📄 RAG Based pdf chatbot

![RAG Based pdf chatbot]

**RAG Based pdf chatbot** is a powerful Streamlit-based application designed to simplify document management. Upload your PDF documents, create embeddings for efficient retrieval, and interact with your documents through an intelligent chatbot interface. Although due to lack of time, I think this is not completed yet because some more features will make this application much better.

- **Upload Documents**: Easily upload and preview your PDF documents within the app.
- **Create Embeddings**: Generate embeddings for your documents to enable efficient search and retrieval.
- **Chatbot Interface**: Interact with your documents using a smart chatbot that leverages the created embeddings.

## 🖥️ Tech Stack

- **[LangChain]**: It is Utilized as the orchestration framework to manage the flow between different components, including embeddings creation, vector storage, and chatbot interactions.
- **[Unstructured]**: Employed for robust PDF processing, enabling the extraction and preprocessing of text from uploaded PDF documents.
- **[BGE Embeddings from HuggingFace]**: Used to generate high-quality embeddings for the processed documents, facilitating effective semantic search and retrieval.
- **[Qdrant]**: A vector database running locally via Docker, responsible for storing and managing the generated embeddings for fast and scalable retrieval.
- **[LLaMA 3.2 via Ollama]**: Integrated as the local language model to power the chatbot, providing intelligent and context-aware responses based on the document embeddings.
- **[Streamlit]**: The core framework for building the interactive web application, offering an intuitive interface for users to upload documents, create embeddings, and interact with the chatbot.

**Future considerations**
1.) When I was going some research papers, I found out that instead of having a sequential flow of data we can make all preprocessing in parallel. This will allow to handle large pdf with many P&L tables.

2.) Implement advanced prompt engineering and few-shot learning techniques to improve response quality.

3.) Implemention of multilingual support for global enterprises handling financial data in different languages.

4.) Support of voice-based financial queries using speech-to-text models.

5.) Allow real-time financial trend analysis and anomaly detection in P&L statements.

6.) Also Integration of financial forecasting models (e.g., ARIMA, LSTMs, Transformer-based models) for predictive insights will make the application muuch better.

## 📁 Directory Structure

RAG_Based_pdf_chatbot/

```
│── logo.png
├── new.py
├── vectors.py
├── chatbot.py
├── requirements.txt
```

## 🚀 Getting Started

Follow these instructions to set up .

### 1. Clone the Repository

```bash

1. Create a Virtual Environment

You can either use Python’s venv or Anaconda to create a virtual environment for managing dependencies.

Option 1: Using venv

On Windows:

python -m venv venv
venv\Scripts\activate

On macOS and Linux:

python3 -m venv venv
source venv/bin/activate

Option 2: Using Anaconda

Follow these steps to create a virtual environment using Anaconda:

	1.	Open the Anaconda Prompt.
	2.	Create a new environment:

conda create --name RAG_Based_pdf_chatbot python=3.9

	3.	Activate the newly created environment:

conda activate RAG Based pdf chatbot



2. Install Dependencies

Once the environment is set up (whether venv or Conda), install the required dependencies using requirements.txt:

pip install -r requirements.txt



```
