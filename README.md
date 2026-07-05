# Local AI Code Assistant

A local AI-powered coding assistant built with **Ollama**, **Qwen2.5-Coder**, **Gradio**, and the **OpenAI-compatible API**.

The application enables developers to chat with a locally hosted Large Language Model (LLM), upload source code files, and receive AI-assisted explanations, code analysis, and programming guidance through an interactive web interface.

---

# Project Overview

AI coding assistants have become an essential tool for software development. However, many existing solutions rely on cloud-hosted models, requiring users to upload proprietary source code to external services.

This project demonstrates how to build a **fully local AI Code Assistant** that allows developers to analyze source code while keeping their data on their own machine.

The assistant combines a conversational interface with code file uploads, enabling users to ask questions about their code, request explanations, identify potential issues, and better understand existing implementations.

---

# Business Problem

Developers frequently need assistance with:

- Understanding unfamiliar code
- Explaining complex functions
- Reviewing implementation logic
- Debugging programming issues
- Learning new programming languages

Uploading proprietary source code to cloud-based AI services may not always be desirable due to privacy or security concerns.

This project demonstrates how these challenges can be addressed using a **locally hosted Large Language Model** powered by Ollama.

---

# Key Features

- Local AI inference using Ollama
- Qwen2.5-Coder language model
- Interactive Gradio web interface
- Code file upload and analysis
- Conversational AI interface
- Chat history preservation
- OpenAI-compatible API integration
- Support for multiple programming languages

Supported file types include:

- Python
- JavaScript
- Java
- C++
- Shell Scripts
- Text Files

---

# Application Interface

The Gradio interface allows users to chat with the AI assistant while optionally uploading source code files for analysis.

<img width="1755" height="983" alt="Example_display" src="https://github.com/user-attachments/assets/b1f310b0-bac3-4b0e-9421-41f4254bdbc6" />


---

# Demo

Example interaction with the Local AI Code Assistant.

The assistant receives a code file, understands the uploaded content, and generates context-aware explanations using Qwen2.5-Coder running locally through Ollama.

<img width="800" height="450" alt="SuperSlowCodingDemo" src="https://github.com/user-attachments/assets/c2a83c95-c900-4366-a76b-0421108893ca" />


---

# Technology Stack

## Artificial Intelligence

- Ollama
- Qwen2.5-Coder
- OpenAI Python SDK

## Frontend

- Gradio

## Backend

- Python

## Development Tools

- VS Code
- Git
- Virtual Environment

---

# System Workflow

The application follows a simple conversational workflow.

1. The user enters a programming question or uploads a source code file.
2. The uploaded file is read by the Gradio application.
3. The file content and user prompt are formatted into a request.
4. The request is sent to Ollama using the OpenAI-compatible API.
5. Qwen2.5-Coder analyzes the code and generates a response.
6. The assistant returns the response while maintaining the conversation history.

---

# Repository Structure

```text
Local-AI-Code-Assistant/

├── README.md
├── gradio_app.py
├── ollama_chat.py
├── on_start.sh
├── requirements.txt
├── LICENSE
├── .gitignore
├── interface.png
└── demo.gif
```

---

# Installation

## Clone the repository

```bash
git clone https://github.com/AShirsat96/Local-AI-Code-Assistant.git
cd Local-AI-Code-Assistant
```

---

## Install dependencies

```bash
pip install -r requirements.txt
```

---

## Install Ollama

Download and install Ollama from:

https://ollama.com/download

---

## Download the model

```bash
ollama pull qwen2.5-coder
```

---

## Start Ollama

```bash
ollama serve
```

---

## Launch the application

```bash
python gradio_app.py
```

Open your browser and navigate to:

```
http://127.0.0.1:7860
```

---

# Skills Demonstrated

This project demonstrates practical experience with:

- Local LLM deployment
- AI-powered developer tools
- Conversational AI
- Code understanding using LLMs
- OpenAI-compatible APIs
- Gradio application development
- Python application development
- Prompt engineering
- Software engineering workflows

---

# Future Improvements

Potential enhancements include:

- Multi-file project analysis
- Repository-level code understanding
- Syntax highlighting
- Streaming responses
- Model selection from the UI
- Docker deployment
- Support for additional programming languages
- Retrieval-Augmented Generation (RAG) for large codebases

---

# About the Author

**Aniket Shirsat**

AI Engineer | Data Scientist | Generative AI

- LinkedIn: https://www.linkedin.com/in/aniketshirsatsg/
- GitHub: https://github.com/AShirsat96
- Portfolio: https://aniketdshirsat.com

---

# License

This project is licensed under the MIT License.
