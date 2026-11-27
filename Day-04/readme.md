# Day 4 – Smart Grocery Shopping Assistant

## Project Overview

The Smart Grocery Shopping Assistant is an AI-powered chatbot designed to help customers with basic grocery shopping activities. It can provide product prices, calculate total costs, check store timings, and record customer orders.

This project was developed as part of the Day 4 Agentic AI task, focusing on **Tools, Structured Output, Pydantic, Google Sheets, and LangChain Agents**.

## Technologies Used

- Python
- LangChain
- Groq API
- Google Colab
- Pydantic
- Google Sheets
- gspread

## Features

1. **Product Price Checking:** Provides the price of available grocery products.
2. **Total Price Calculation:** Calculates the total amount based on the selected product and quantity.
3. **Store Timings:** Checks the store's working hours for different days.
4. **Order Management:** Collects customer details and grocery order information.
5. **Structured Output:** Uses Pydantic to extract and validate order details.
6. **Google Sheets Integration:** Saves customer orders in a Google Sheet for record keeping.
7. **AI Agent:** Uses a LangChain agent to understand customer requests and select the appropriate tools.

## Available Grocery Products

The assistant uses a sample product catalogue containing:

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

## Tools Implemented

The project includes three main tools:

- `get_price()` – Checks product prices and calculates the total amount.
- `is_open()` – Provides the store's opening and closing timings.
- `log_order()` – Validates order details and stores the order in Google Sheets.

## Structured Output and Validation

Pydantic is used to define an Order model with the following fields:

- Customer name
- Product name
- Quantity
- Requested date

It also validates the product selection and ensures that the quantity is at least 1.

## Google Sheets Integration

Google Sheets is used to store customer orders automatically.

Each order contains:

- Customer Name
- Product
- Quantity
- Unit
- Requested Date
- Total Price

This makes it easier to maintain and view customer order records.

## How to Run the Project

1. Open the project notebook in Google Colab.
2. Install the required Python libraries.
3. Add the Groq API key to Colab Secrets using the name `GROQ_API_KEY`.
4. Run the notebook cells.
5. Complete Google account authentication when prompted.
6. Start interacting with the grocery shopping assistant.
7. Check Google Sheets to view the saved orders.

## Sample Questions to Test

- What is the price of 2 kg rice?
- Calculate the cost of 3 litres of milk.
- What are the store timings on Sunday?
- What is the price of apples?
- I want to place an order for 2 kg rice.
- Can you save my grocery order?

## Learning Outcomes

Through this task, I learned how to:

- Create tools for an AI agent.
- Use Pydantic for structured data validation.
- Integrate Google Sheets with Python.
- Build an AI agent using LangChain.
- Connect an LLM with external tools.
- Maintain customer order information.

## Conclusion

This project demonstrates how an AI agent can do more than simply answer questions. By connecting an LLM with Python tools and Google Sheets, the Smart Grocery Shopping Assistant can perform useful grocery-related tasks and manage customer orders.