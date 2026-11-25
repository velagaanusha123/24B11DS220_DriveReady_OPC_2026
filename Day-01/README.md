# AI Personal Assistant Using Groq API

## About the Project

This project is a simple AI personal assistant developed as part of my AI Agents workshop. The main aim is to understand how Large Language Models (LLMs) work and how they can be integrated into Python applications using APIs.

The assistant accepts questions from users and generates responses using the Groq API. I used LangChain to connect the application with the AI model and created an interactive program using Python.

## Technologies Used

- Python
- LangChain
- Groq API
- Google Colab
- GPT-OSS-20B Model

## Implementation

First, I installed the required LangChain Groq package in Google Colab. Then, I created a Groq API key and stored it securely in Google Colab Secrets using the name `GROQ_API_KEY`.

After setting up the API connection, I initialized the language model using LangChain. The program accepts user input, sends the prompt to the AI model, and displays the generated response.

I also added an exit option so users can end the conversation whenever they want.

## How to Run

1. Open the Python notebook in Google Colab.
2. Install the required package:

   `!pip install -q langchain-groq`

3. Create a Groq API key from https://console.groq.com/keys.
4. Open Secrets in Google Colab and add your API key with the name `GROQ_API_KEY`.
5. Enable notebook access for the secret.
6. Run the code cells and start interacting with the assistant.

Type `exit`, `quit`, or `bye` to stop the assistant.

## Sample Output

    Welcome to AI Personal Assistant

    You: What is Artificial Intelligence?

    Assistant: Artificial Intelligence is the ability of
    machines to perform tasks that normally require
    human intelligence.

    You: exit

    Assistant: Goodbye! Have a great day!

## What I Learned

Through this project, I learned how to connect Python applications with AI models using APIs. I also gained practical experience with LangChain, Gro