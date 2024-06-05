# Gemini Quizzify

![Image](https://github.com/ruhi47/gemini-quizzify/blob/main/gemini-quizzify.jpg) 

## Welcome to Gemini Quizzify
an intelligent and interactive quiz generation application built to transform documents into engaging quizzes. Whether you're an educator, a student, or a knowledge enthusiast, Gemini Quizzify makes it simple and fun to test and improve your understanding of any topic.

## About the Project

Gemini Quizzify leverages the power of Natural Language Processing (NLP) and machine learning to convert your documents into quizzes. It's designed to help users create, manage, and take quizzes effortlessly, providing an interactive way to reinforce learning.

## Features

- Document Ingestion: Easily upload PDF documents for quiz generation.
- Intelligent Quiz Generation: Generate quizzes based on the content of the uploaded documents using advanced NLP techniques.
- User-Friendly Interface: A sleek and intuitive UI built with Streamlit for seamless user experience.
- Session Management: Maintain quiz progress and handle user interactions effectively.
- Customizable: Configure the number of questions and topics for tailored quizzes.

## Installation
To get started with Gemini Quizzify, follow these steps:

1. Clone the Repository:
```
git clone https://github.com/ruhi47/gemini-quizzify.git
cd gemini-quizzify
```
2. Create and Activate a Virtual Environment:
```
python3 -m venv env
source env/bin/activate
```
3. Install Dependencies:
```
pip install -r requirements.txt
```
## Usage

1. Run the Streamlit App:
```
streamlit run tasks/task_10/task_10.py
```
2. Interact with the Application:
3. Upload PDF documents.
4. Enter the topic for the quiz.
5. Specify the number of questions.
6. Generate and take the quiz.

## How It Works

- **Document Ingestion:**
The DocumentProcessor class handles the ingestion of PDF documents, extracting text and preparing it for quiz generation.

- **Embedding and Chroma Collection:** 
Using the EmbeddingClient, the text from the documents is embedded using a pre-trained model. The ChromaCollectionCreator organizes these embeddings into a searchable collection.

- **Quiz Generation:** 
The QuizGenerator takes the embedded collection and the specified topic to generate relevant quiz questions. Questions are crafted to cover key concepts and details from the document.

- **Quiz Management:** 
The QuizManager handles the display and navigation of quiz questions, ensuring a smooth user experience. It keeps track of the current question index and manages user interactions.

## Configuration

- Embedding Configuration
Edit the embed_config dictionary in task_10.py to configure the embedding client:
```
embed_config = {
    "model_name": "textembedding-gecko@003",
    "project": "YOUR-PROJECT-ID-HERE",
    "location": "us-central1"
}
```
- Session State
The session state is used to manage the quiz state. Ensure that your app initializes and updates session state variables correctly to maintain quiz progress.

## Contributing

We welcome contributions to improve Gemini Quizzify! To contribute:

1. Fork the repository.
2. Create a new branch for your feature (git checkout -b feature/YourFeature).
3. Commit your changes (git commit -m 'Add some feature').
4. Push to the branch (git push origin feature/YourFeature).
5. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

# Mission Quizify

## Technology Stack

- ![Streamlit](https://img.shields.io/badge/Framework-Streamlit-brightgreen)
- ![Python](https://img.shields.io/badge/Language-Python-blue)
- ![Google Cloud AI](https://img.shields.io/badge/ML-Google%20Cloud%20AI-yellow)
- ![Streamlit](https://img.shields.io/badge/Streamlit-Open%20Source-FF4B4B?logo=streamlit)
- ![Chromadb](https://img.shields.io/badge/Chromadb-Database-4285F4?logo=chromadb)
- ![Langchain](https://img.shields.io/badge/Langchain-Blockchain-FFA700?logo=langchain)
- ![Langchain Google VertexAI](https://img.shields.io/badge/Langchain%20Google%20VertexAI-Machine%20Learning-4285F4?logo=google-cloud)
- ![PyPDF](https://img.shields.io/badge/PyPDF-Library-3776AB?logo=python)

## Development Tools

- ![Virtualenv](https://img.shields.io/badge/Environment-Virtualenv-blueviolet)
- ![Git](https://img.shields.io/badge/Version%20Control-Git-red)
- ![GitHub](https://img.shields.io/badge/Repository-GitHub-lightgrey)

## Acknowledgements

Streamlit for providing an excellent framework for building interactive web apps.
OpenAI for developing the powerful language models that make intelligent quiz generation possible.
The open-source community for continuous contributions and improvements.
