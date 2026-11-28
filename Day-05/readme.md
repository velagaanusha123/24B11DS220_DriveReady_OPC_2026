# Day 5 - Smart Grocery Shopping Assistant

## Project Overview

The Smart Grocery Shopping Assistant is a chatbot designed to make grocery shopping easier for customers. It helps users check product prices, get information about available groceries, calculate shopping costs, and place orders through a simple conversation.

This project was developed as part of the Day 5 Agentic AI task.

## Technologies Used

- Python
- LangChain
- LangGraph
- Groq API
- ChromaDB
- Google Colab

## Features

- **Product Price Checking:** Customers can ask for the prices of grocery products and calculate the total cost based on quantity.
- **Product Information:** The assistant provides information about available grocery items.
- **RAG Implementation:** ChromaDB is used as a vector database to store and retrieve relevant information from the grocery knowledge base.
- **Tool Integration:** The assistant uses different tools to check prices, search information, check store details, and save orders.
- **Conversational Memory:** The chatbot remembers previous messages during a conversation and can respond using the stored context.
- **Order Management:** Customers can prepare and confirm grocery orders. Confirmed orders are saved in a CSV file.

## Grocery Products

The assistant currently supports the following products:

| Product | Price |
|---|---:|
| Rice | ₹60/kg |
| Sugar | ₹45/kg |
| Milk | ₹30/litre |
| Bread | ₹40/packet |
| Eggs | ₹7/piece |
| Apples | ₹120/kg |
| Tomatoes | ₹35/kg |
| Potatoes | ₹30/kg |
| Oil | ₹150/litre |

## How It Works

1. The user enters a question or request in the chatbot.
2. The Groq language model understands the user's request.
3. The agent selects the appropriate tool when required.
4. ChromaDB retrieves relevant information from the knowledge base for information-based questions.
5. The assistant generates a response and maintains conversation context.
6. Confirmed grocery orders are stored in a CSV file.

## How to Run

1. Open the project notebook in Google Colab.
2. Install the required Python packages.
3. Add the Groq API key as `GROQ_API_KEY` in Colab Secrets.
4. Run the notebook cells.
5. Start interacting with the Smart Grocery Shopping Assistant.

## Example Questions

- What is the price of 2 kg rice?
- How much will 3 litres of oil cost?
- What grocery products are available?
- What is the price of 5 eggs?
- My name is Anusha. What is my name?
- I want to order rice and milk.

## Learning Outcomes

Through this task, I learned how to build an AI agent using LangChain and LangGraph, integrate tools with a language model, use ChromaDB for retrieving relevant information, and maintain conversational memory.

## Conclusion

This project helped me understand how an AI assistant can do more than just answer questions. By combining an LLM, tools, a knowledge base, and memory, the Smart Grocery Shopping Assistant can support customers with everyday grocery shopping activities.