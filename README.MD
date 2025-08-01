
# MedicalRAG.py

---

A multimodal Retrieval-Augmented Generation (RAG) pipeline designed to analyze veterinary medical documents, with a specific focus on dog health. This script uses cutting-edge language models, document parsing tools, and vector search technologies to provide advanced question answering and summarization capabilities.

## Features

* **PDF Parsing:** Extracts text, tables, and images from PDF files using the `unstructured` library.
* **Summarization:** Uses Google Gemini LLMs to summarize each extracted element (text, table, and image).
* **Image Analysis:** Processes and encodes images with Gemini's vision model to generate content descriptions.
* **Vector Store:** Stores all summaries and metadata in a FAISS vector database for efficient similarity search and retrieval.
* **Question Answering:** Answers user queries about dog health by retrieving relevant context from the vector database and providing multimodal responses (text, tables, and images).
* **Colab Integration:** Designed for seamless use in Google Colab, including API key management via `Colab’s userdata`.

---

## Dependencies

This project relies on the following key libraries and tools:

* **Python Libraries:**
    * `LangChain`
    * `Google Generative AI`
    * `FAISS`
    * `unstructured`
* **System Dependencies:**
    * `Tesseract OCR`
    * `Poppler Utils`

---

## Usage

This script is designed to be used in a Google Colab environment.

1.  **Install Dependencies:** Ensure all required Python libraries and system dependencies (`Tesseract`, `Poppler`) are installed in your environment.
2.  **Extract Elements:** The script will automatically extract text, tables, and images from a specified veterinary PDF.
3.  **Summarize and Store:** Each extracted element is summarized using Gemini models and stored in a FAISS vector store.
4.  **Ask Questions:** You can then ask questions about the document. The script retrieves the most relevant context and generates a detailed, evidence-based answer.

### Example

Given a veterinary PDF, you can ask a question like:
The script will retrieve the relevant text, tables, and images and provide a detailed, model-generated answer. It can even display annotated images to support its response.

![image alt](https://github.com/priyank766/Multimodel_RAG/blob/main/Screenshot%202025-08-01%20222314.png)

# **"What is Gingivitis?"**

![image alt](https://github.com/priyank766/Multimodel_RAG/blob/main/Screenshot%202025-08-01%20222421.png)

---

## Contributing

For any suggestions or issues, please open an issue in the repository.
