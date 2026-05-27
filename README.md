# Retrieval-Augmented Generation (RAG) Demonstration

A generic demonstration of Retrieval-Augmented Generation (RAG) using locally hosted models via Ollama. The restaurant review example is just one specific use case to showcase the implementation.

## Overview

This project demonstrates a minimal RAG pipeline to answer questions based on provided data examples using:
- Local LLMs (via Ollama)
- Embedding models (via Ollama)
- Vector storage (ChromaDB)

## Setup Instructions

### 1. Prerquisites
- [Install Ollama](https://ollama.ai) (macOS: `brew install ollama`)
- [Install Python](https://python.org) (3.9+ recommended)

### 2. Create Virtual Environment
```bash
# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 3. Ollama Setup
```bash
# Start Ollama server
ollama serve

# Pull required models
ollama pull llama3.2
ollama pull mxbai-embed-large
```

### 4. Project Launch
```bash
python main.py
```

## Usage

Enter questions based on provided data examples when prompted. Type `exit` to quit. While this example uses restaurant reviews, you can swap datasets by moving your own CSV/JSON files into the project directory.

## Notes

- All models run locally via Ollama
- Virtual environment ensures dependency isolation
- ChromaDB stores embeddings locally in `chroma_langchain_db`
- This implementation is intentionally generic - replace the `realistic_restaurant_reviews.csv` with your own data source to adapt to other domains.

A simple **Retrieval-Augmented Generation (RAG)** demonstration using locally hosted models via Ollama.

## Overview

This project shows how to build a minimal RAG pipeline to answer questions about restaurant reviews using:
- Local LLMs (via Ollama)
- Embedding models (via Ollama)
- Vector storage (ChromaDB)

## Setup Instructions

### 1. Prerquisites
- [Install Ollama](https://ollama.ai) (macOS: `brew install ollama`)
- [Install Python](https://python.org) (3.9+ recommended)

### 2. Create Virtual Environment
```bash
# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 3. Ollama Setup
```bash
# Start Ollama server
ollama serve

# Pull required models
ollama pull llama3.2
ollama pull mxbai-embed-large
```

### 4. Project Launch
```bash
python main.py
```

## Usage

Enter questions about restaurant reviews when prompted. Type `exit` to quit.

## Notes

- All models run locally via Ollama
- Virtual environment ensures dependency isolation
- ChromaDB stores embeddings locally in `chroma_langchain_db`