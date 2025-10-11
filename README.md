# RAG-based PDF Chatbot with IBM Watsonx and LangChain

This project is a **Retrieval-Augmented Generation (RAG) chatbot** that allows users to upload a PDF document and ask questions. The chatbot leverages **IBM Watsonx AI models** for language understanding and **LangChain** for document processing and vector retrieval.


## Features

- Upload a PDF and ask natural language questions.
- Uses **IBM Watsonx** for:
  - Text generation (`mixtral-8x7b-instruct-v01`)
  - Text embeddings (`slate-125m-english-rtrvr`)
- Uses **LangChain** for:
  - Document loading
  - Text splitting into chunks
  - Vector database and retrieval
- Gradio interface for an easy-to-use web app.
- Returns both answers and source documents.


## Installation

1. Clone this repository:

```bash
git clone https://github.com/NakadBellon/RAG-based-PDF-Chatbot-with-IBM-Watsonx-and-LangChain.git
cd RAG-based-PDF-Chatbot-with-IBM-Watsonx-and-LangChain
```

2. Install the required packages:
`pip install ibm-watsonx-ai langchain langchain-ibm langchain-community gradio`

You might also need chromadb if not installed automatically:
`pip install chromadb`

## Usage

1. Launch the chatbot:
`python rag_chatbot.py`
2. Open the link displayed by Gradio in your browser.
3. Upload a PDF file and type your query.
4. The chatbot will return the answer and the source text.

## File structure

  - rag_chatbot.py: "Main Python script for the chatbot."
  - README.md: "Project documentation."
  - .gitignore: "Git ignore rules."
  - LICENSE: "Project license file."

## License

  name: "MIT License"
  details: "See the LICENSE file for details."

## acknowledgements:
  - "IBM Watsonx"
  - "LangChain"
  - "Gradio"


