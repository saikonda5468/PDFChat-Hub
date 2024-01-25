# PDFChat Hub



## Overview
------------
Welcome to PDFChat Hub! This Python application enables you to engage in conversations with multiple PDF documents. By posing questions in natural language, you can receive insightful responses based on the content of the PDFs. The app leverages advanced language models to provide accurate and contextually relevant answers. Remember, PDFChat Hub responds exclusively to questions related to the loaded PDFs.

## How It Operates
------------

![PDFChat Hub Diagram](./docs/PDF-LangChain.jpg)

PDFChat Hub functions through the following key steps to offer responses to your queries:

1. **PDF Loading:** The app reads and processes multiple PDF documents, extracting their textual content.

2. **Text Chunking:** Extracted text undergoes segmentation into manageable chunks for effective processing.

3. **Language Model:** The application employs a sophisticated language model to generate vector representations (embeddings) of the text chunks.

4. **Similarity Matching:** When you ask a question, the app compares it with the text chunks, identifying the most semantically similar ones.

5. **Response Generation:** The selected chunks are fed into the language model, which produces a response based on the pertinent content of the PDFs.

## Installation and Dependencies
----------------------------
Get PDFChat Hub up and running by following these installation steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by executing the following command:
   ```
   pip install -r requirements.txt
   ```

3. Acquire an API key from OpenAI and insert it into the `.env` file in the project directory.
```commandline
OPENAI_API_KEY=your_secret_api_key
```

## Usage
-----
Explore the capabilities of PDFChat Hub with these usage instructions:

1. Confirm the installation of necessary dependencies and ensure the OpenAI API key is added to the `.env` file.

2. Launch the application by running the `main.py` file through the Streamlit CLI. Use the following command:
   ```
   streamlit run app.py
   ```

3. The application will open in your default web browser, showcasing the user-friendly interface.

4. Load multiple PDF documents into the app following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.

