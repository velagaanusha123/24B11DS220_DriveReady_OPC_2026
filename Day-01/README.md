# NovaAI – AI Personal Assistant

## About the Project

NovaAI is a simple AI personal assistant developed as part of my AI Agents workshop. The main aim of this project is to understand how Large Language Models (LLMs) work and how they can be integrated into Python applications using APIs.

NovaAI accepts questions from users and generates responses using the Groq API. I used LangChain to connect the application with the AI model and created a simple interactive interface in Google Colab.

## Technologies Used

- Python
- LangChain
- Groq API
- Google Colab
- GPT-OSS-20B Model

## Implementation

First, I installed the required LangChain Groq package in Google Colab. Then, I created a Groq API key and stored it securely in Google Colab Secrets.

After setting up the API connection, I initialized the language model using LangChain. I created a simple program that accepts user input, sends the prompt to the AI model, and displays the generated response.

I also added an exit option so that users can end the conversation whenever they want.

## How to Run

1. Open the `NovaAI.ipynb` notebook in Google Colab.
2. Install the required package:

   `!pip install -q langchain-groq`

3. Create a Groq API key from https://console.groq.com/keys.
4. Store the API key in Google Colab Secrets with the name `GROQ_API_KEY`.
5. Enable notebook access for the secret.
6. Run the code cells and start interacting with NovaAI.

Type `exit`, `quit`, or `bye` to stop the assistant.

## Sample Output

    Welcome to NovaAI
    Your Personal AI Assistant

    You: What is Artificial Intelligence?

    NovaAI: Artificial Intelligence is the ability of
    machines to perform tasks that normally require
    human intelligence.

    You: exit

    NovaAI: Goodbye! Have a great day!

## What I Learned

Through this project, I learned how to connect Python applications with AI models using APIs. I also gained practical experience with LangChain, Groq, user prompts, and Large Language Models.

## Future Improvements

- Add conversation history and memory.
- Develop a simple web-based interface.
- Include voice-based interaction.
- Improve the assistant with additional features.

## Author

Anusha

---

This project was developed for learning and educational purposes as part of an AI Agents workshop.