# Smart Grocery Shopping Assistant

## Project Overview

The Smart Grocery Shopping Assistant is a conversational AI chatbot developed as part of the Day 2 AI Agents Workshop.

The application helps users get grocery product information, check prices, calculate product costs, and discuss their shopping requirements through a natural language interface.

It uses Python and the Groq API to generate responses and maintain conversation history.

## Objectives

- Develop a conversational grocery shopping assistant.
- Provide product information using a predefined catalogue.
- Calculate grocery prices based on quantity.
- Maintain conversation history.
- Understand and classify customer messages.
- Extract shopping information in JSON format.

## Features

1. **Product Catalogue:** Stores grocery products, prices, and units using a Python dictionary.
2. **Price Calculation:** Calculates the total price of a product based on the requested quantity.
3. **System Prompt:** Uses Role, Facts, Rules, and Format to guide chatbot responses.
4. **Function Logging:** Uses a Python decorator to log function calls and results.
5. **Conversation Memory:** Maintains previous user and assistant messages during a conversation.
6. **Error Handling:** Handles API connection errors, rate limits, and other exceptions.
7. **Few-Shot Classification:** Classifies customer messages into product queries, price queries, shopping-list requests, and other messages.
8. **JSON Extraction:** Extracts customer names, grocery items, quantities, and budgets into structured JSON data.

## Technologies Used

- Python
- Google Colab
- Groq API
- OpenAI Python Library
- JSON

## Sample Product Catalogue

| Product | Price | Unit |
|---|---:|---|
| Rice | ₹60 | kg |
| Sugar | ₹45 | kg |
| Milk | ₹30 | litre |
| Bread | ₹40 | packet |
| Eggs | ₹7 | piece |
| Apples | ₹120 | kg |
| Tomatoes | ₹35 | kg |
| Potatoes | ₹30 | kg |
| Oil | ₹150 | litre |

*Note: These are sample prices used for demonstration purposes.*

## How to Run the Project

1. Open the notebook using Google Colab.
2. Install the required OpenAI Python library.
3. Add your Groq API key to Google Colab Secrets using the name `GROQ_API_KEY`.
4. Enable notebook access to the secret.
5. Run the notebook.
6. Interact with the Smart Grocery Shopping Assistant using the input prompt.

## Workshop Activities Completed

- Activity 1: System prompt experiment.
- Activity 2: Few-shot message classification.
- Activity 3: Grocery order extraction using JSON.
- Activity 4: Conversation memory experiment.
- Activity 5: Implementation of a custom grocery shopping use case.

## Sample Test Questions

- What grocery products are available?
- What is the price of rice?
- Calculate the cost of 3 kg rice.
- Add milk and bread to my shopping list.
- Can I buy these items within ₹200?
- What items did I ask for?
- Do you sell chocolate?

## Project Limitations

- Product prices are predefined sample values.
- The application does not use live supermarket inventory.
- It does not place real grocery orders or process payments.
- Conversation history is maintained during the current session and is not permanently stored.
- The chatbot does not automatically execute the separate price calculation function for every natural language request.

## Future Enhancements

- Integrate a database to store customer shopping lists.
- Add live product availability and pricing.
- Develop a web-based user interface.
- Add budget-based grocery recommendations.
- Implement a functional shopping cart and order management system.

## Learning Outcomes

Through this project, I learned about system prompting, Python dictionaries, functions, decorators, exception handling, few-shot learning, JSON processing, and conversation memory. I also understood how an AI model can be connected to a Python application using an API.

## Conclusion

The Smart Grocery Shopping Assistant demonstrates the basic concepts of conversational AI using a practical grocery shopping use case. This project provided hands-on experience with the fundamental building blocks used in developing AI assistants and agents.