# Emotion Detection Application Using IBM Watson and Flask

This project is an emotion detection application using IBM Watson's Natural Language Understanding (NLU) service. The application is built with Flask for web deployment and includes unit tests and error handling.

## Table of Contents
- Project Structure
- Setup Instructions
- Usage
- Error Handling
- Static Code Analysis
- License

## Project Structure

Practice-Repository/
├── my_emotion_app/
│   ├── __init__.py
│   └── emotion_detector.py
├── server.py
├── test_emotion_detector.py
├── test_script.py
└── README.md

## Setup Instructions

    Clone the repository:

    git clone https://github.com/Shaikh-Hammad947/Practice-Repository.git
    cd Practice-Repository

    Install dependencies:

    pip install -r requirements.txt

    Set up environment variables:
        Create a .env file in the project root and add your IBM Watson API key and URL:

    Run the application:

    python server.py

    Run unit tests:

    python -m unittest discover

    Run static code analysis:

    flake8 server.py

## Usage

    Send a POST request to the /predict endpoint with a JSON payload containing the text to analyze:

    curl -X POST http://127.0.0.1:5000/predict -H "Content-Type: application/json" -d '{"text": "I am very happy today!"}'

## Error Handling

    The application handles cases where no text is provided and returns a 400 Bad Request status with an error message.

## Static Code Analysis

    The project uses flake8 for static code analysis to ensure code quality and adherence to PEP 8 standards.

## License

This project is licensed under the MIT License.
