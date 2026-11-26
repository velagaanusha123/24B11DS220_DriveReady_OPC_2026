# Smart Grocery Shopping Assistant – Day 3

## Project Overview

The Smart Grocery Shopping Assistant is a conversational AI application developed as part of the Day 3 Agentic AI Workshop.

This project uses LangChain and the Groq API to create a chatbot that answers grocery-related questions using a predefined product catalogue. It demonstrates prompt templates, conversation memory, LLM chains, automated testing and the basic LangChain agent interface.

## Features

- Grocery product catalogue using Python dictionaries.
- LangChain prompt templates.
- Groq language model integration.
- Conversation history and memory.
- LangChain chains using output parsers.
- Automated chatbot testing using `tests.csv`.
- Prompt improvement and pass-rate comparison.
- Temperature experiment.
- LangChain agent preview.
- Python functions prepared for future agent tools.

## Technologies Used

- Python
- Google Colab
- LangChain
- LangChain-Groq
- Groq API
- CSV

## Implementation

The application uses `ChatPromptTemplate` to structure messages and `MessagesPlaceholder` to maintain conversation history. The prompt, language model and `StrOutputParser` are connected using the LangChain pipe operator to create a chain.

The chatbot is evaluated using ten grocery-related customer questions stored in `tests.csv`. Each test includes an expected phrase, which is used to calculate the pass rate.

## Workshop Activities

1. Created the grocery assistant using LangChain.
2. Implemented customer conversation history.
3. Created automated tests for chatbot responses.
4. Compared original and improved system prompts.
5. Tested response variation using temperature 1.0.
6. Classified grocery business tasks as traditional software, generative AI or agentic AI.
7. Created a basic LangChain agent preview.
8. Prepared two Python functions for Day 4 tool integration.

## How to Run

1. Open the notebook in Google Colab.
2. Add your Groq API key to Colab Secrets as `GROQ_API_KEY`.
3. Enable notebook access to the secret.
4. Run the notebook code.
5. Review the automated test results.
6. Interact with the grocery assistant.

## Limitations

- Product prices are sample demonstration data.
- The application does not access live grocery inventory.
- It does not place real orders or process payments.
- The agent preview currently has no connected tools.
- Conversation history is maintained only during the current session.

## Conclusion

This project helped me understand how LangChain can be used to develop conversational AI applications. I learned about prompt templates, LLM chains, output parsers, conversation memory, automated testing and the basic structure of an AI agent. The two prepared Python functions will be used as tools in the next stage of the workshop.