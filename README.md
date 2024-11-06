# FealtyX

This is a project built with FastAPI and Streamlit, integrated with Ollama for AI-powered text generation. The system allows you to manage students, create new students, update student details, delete students, and generate AI-based summaries for students.

## Features
CRUD Operations: Create, Read, Update, and Delete student records.

AI Summary Generation: Use Ollama's Llama model to generate summaries based on student information.

Streamlit Frontend: Provides an interactive UI to manage students and view summaries.

## Prerequisites
Before running the project, ensure you have the following installed:

-> Python 3.x

-> FastAPI

-> Streamlit

-> Requests

-> Ollama (https://github.com/ollama/ollama/blob/main/README.md#quickstart, also install the Llama3 language model for Ollama)

## Installation
Clone the repository and install the following dependencies:

```bash
pip install fastapi uvicorn requests pydantic pandas
```

## Running the project

Open up the Ollama app and type the following command to run Llama model:
```bash
ollama run llama3.2
```

Start the FastAPI backend:
```python
uvicorn main:app --reload
```
Run the Streamlit frontend:
```python
streamlit run app.py
```
Open the Streamlit app in your browser (typically available at http://localhost:8501).

## Usage
Create a New Student: Fill out the form with student details (ID, Name, Age, Email) to create a new student.

Update a Student: Modify the details of an existing student by providing the student ID and the new details.

Delete a Student: Provide the student ID to remove a student from the system.

Generate Summary: For each student, generate an AI-powered summary using Ollama.
