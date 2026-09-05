# AI Expense Tracker Agent

An agentic AI application built using Google's Gemini API with function calling. 
The agent understands natural language expense-related queries, autonomously 
decides which function to call, and takes appropriate action — logging new 
expenses or retrieving spending summaries.

## Features
- Logs expenses from natural language input (amount, category, note)
- Answers spending queries with category-wise and total summaries
- Demonstrates agentic decision-making using Gemini's function-calling capability

## Tech Stack
- Google Gemini API (gemini-3.6-flash)
- Python (Google Colab)
- google-genai SDK

## Example Interactions
- "I spent 500 rupees on groceries" → logs expense
- "How much have I spent on food?" → returns category summary
- "What's my total spending?" → returns overall total

## How It Works
The agent uses Gemini's function-calling feature to interpret user intent 
and trigger one of two functions: `log_expense()` or `get_expense_summary()`, 
based on the natural language input — without hardcoded rules.
