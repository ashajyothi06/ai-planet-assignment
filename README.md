# AI PDF Inquire Fullstack 

## React Frontend with LLamaIndex Integration - Retrieval-augmented generation (RAG) App for AIPlanet Assignment.

### https://aipdfinquire.netlify.app/ - Online Hosted
### Frontend Hosted on Netlify and backend on Keyobe. Allows almost all functionallity.
Keyobe Branch altered for hosting, Main branch for local hosting and development.


#### Video Demostration : https://drive.google.com/file/d/1jCAzgZMkt0bYi8UMVkz5jwiH5wbIRXw-/view?usp=sharing

This project demonstrates the integration of a React frontend with a backend server built with FastAPI. It includes features such as uploading PDF files, querying text from PDFs using AI, and managing chat interactions.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Setup](#setup)
  - [Frontend Setup](#frontend-setup)
  - [Backend Setup](#backend-setup)
- [File Structure](#file-structure)
- [Project Outline](#project-outline)
  - [Backend Specification](#backend-specification)
  - [Frontend Specification](#frontend-specification)
- [Contributing](#contributing)
- [License](#license)

## Overview

Developed the AI PDF Inquire Fullstack application, integrating a React frontend with a FastAPI backend to enable AI-driven PDF querying. Leveraged LLamaIndex for Retrieval-Augmented Generation (RAG) and natural language processing, allowing users to upload PDFs and interact with the content through AI. The project features a user-friendly chat interface and robust error handling. Hosted the frontend on Netlify and the backend on Koyeb, demonstrating expertise in full-stack development, RESTful APIs, and AI integration.

## Features

- Upload PDF files
- Extract text content from uploaded PDFs
- Chat interface with a chatbot
- Clear uploaded PDFs and chat messages

## Setup

### Frontend Setup

1. Clone this repository.
2. Navigate to the `react_frontend` directory.
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm start
   ```

### Backend Setup

1. Navigate to the `backend` directory.
2. Create a virtual environment:
   ```bash
   python -m venv venv
   ```
3. Activate the virtual environment:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS and Linux:
     ```bash
     source venv/bin/activate
     ```
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Start the FastAPI server:
   ```bash
   uvicorn main:app --reload
   ```



## Change the origins in the main.py, adding your localhost from Vite.
origins = [
    "http://localhost:5173",  # Your frontend local development URL from Vite
    # Add more origins as needed
]

## File Structure

```
react_frontend/    # React frontend directory
  ├── public/       # Public assets and index.html
  ├── src/          # React source files
  └── ...

my_app/           # FastAPI backend directory
  ├── main.py      # FastAPI application
  └── ...
```

## Project Outline

### Backend Specification

#### FastAPI Endpoints
- **Upload PDF Endpoint**: An endpoint for uploading PDF documents.
- **Query Endpoint**: An endpoint for receiving questions and returning answers based on the uploaded PDFs.

#### PDF Processing
- **Text Extraction**: Extract text from uploaded PDFs using a suitable library
- **NLP Processing**: Use the LLamaIndex to process natural language questions and generate answers based on the PDF content.

#### Data Management
- **Metadata Storage**: Store information about uploaded documents (e.g., filename, upload date) in a database.

### Frontend Specification

#### User Interface
- **Upload PDF**: A page for uploading PDF documents.
- **Question Interface**: A feature for asking questions on uploaded documents and viewing answers.

#### Interactivity
- **Feedback Mechanisms**: Implement feedback mechanisms while uploading documents and processing questions.
- **Error Handling**: Display error messages for unsupported file types or processing errors.
- **Clear Chats**: Allows users to delete indexes and documents uploaded in the backend from the interface.
