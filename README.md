# Sentiment Service Bot
## AI-Powered Customer Service Manager with Sentiment Analytics

This project is a sophisticated Virtual Service Bot developed in a Jupyter Notebook environment. It integrates the Google Gemini API to provide an interactive, context-aware service experience, combined with a data analysis engine that evaluates user satisfaction through sentiment scoring and visual charting.

---

# Project Overview

The Sentiment Service Bot simulates a real-world customer service scenario. It handles live communication, maintains session memory, and performs an "Emotional Audit" to visualize the quality of the interaction. 

The project demonstrates a full implementation of the following core topics:
* Object-Oriented Programming (OOP)
* AI API Integration (LLM)
* Data Persistence (JSON files)
* Advanced Python Logic (Generators and Comprehensions)
* Data Science and Visualization (Matplotlib)

---

# Technical Requirements and Architecture

# 1. Intelligent Conversational Engine
* **ServiceManager Class:** A central OOP structure that manages the entire lifecycle of the bot, from initialization to data analysis.
* **Gemini API Integration:** Implements real-time communication with Google’s Large Language Model, including a custom System Prompt to define the bot’s professional persona.
* **Contextual Memory:** Uses a structured List of Dictionaries to store the full conversation history, ensuring the AI maintains the context of the chat.

# 2. Data Persistence and Storage
* **JSON Serialization:** At the end of every session, the entire conversation history is exported to a structured JSON file.
* **Dynamic Loading:** The system includes a dedicated function to reload JSON logs for post-processing and historical analysis.
* **Exception Handling:** Implements try-except blocks to handle API connectivity issues and File I/O errors (Missing files or saving permissions).

# 3. Sentiment Analysis Engine
* **Data Normalization:** Advanced string manipulation to clean text, remove punctuation, and prepare data for analysis.
* **Custom Sentiment Dictionary:** A domain-specific mapping of positive and negative keywords used to calculate an emotional score for every message.
* **Efficiency:** Leveraging List and Dictionary Comprehensions to perform high-speed text processing and scoring.

---

# Data Visualization and Insights

The project utilizes Matplotlib to transform raw conversation logs into actionable visual insights:

* **Sentiment Trend (Line Chart):** Tracks the cumulative sentiment over time. An upward slope indicates a successful service interaction where the user's mood improved.
* **Tone Comparison (Bar Chart):** Compares the average sentiment of the Bot versus the User, proving the bot’s ability to remain professional regardless of user input.
* **Pain Point Analysis (Bar Chart):** Displays the frequency of specific negative words to identify the main causes of user frustration.

---

# Advanced Python Features Used

* **Generators and Iterators:** Implemented to traverse the conversation history efficiently without high memory overhead.
* **Comprehensions:** Extensive use of List and Dictionary comprehensions for data filtering and sentiment calculation.
* **String Processing:** Usage of built-in string functions for professional text cleaning and formatting.

---

# How to Run

1. Open the recipes.ipynb in Jupyter Notebook or VS Code.
2. Ensure you have a valid Google Gemini API Key configured.
3. Run the cells to start the interactive chat.
4. Type your messages and end the chat by typing "exit" or "quit".
5. View the generated JSON log and the analytical graphs at the end of the notebook.
