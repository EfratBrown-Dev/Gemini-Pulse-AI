# AI-Powered Customer Service Manager with Sentiment Analytics

An AI-powered virtual customer service bot developed in a Jupyter Notebook environment. The project integrates the **Google Gemini API** to provide an interactive, context-aware customer service experience, combined with a sentiment analysis engine that evaluates user satisfaction and visualizes interaction trends.

The project demonstrates the integration of **Object-Oriented Programming, Large Language Models (LLMs), data persistence, text processing, sentiment analysis, and data visualization** in a practical customer service scenario.

---

## Table of Contents

* [Project Overview](#-project-overview)
* [Key Features](#-key-features)
* [Technical Architecture](#-technical-architecture)
* [Data Persistence](#-data-persistence)
* [Sentiment Analysis](#-sentiment-analysis)
* [Data Visualization](#-data-visualization)
* [Advanced Python Features](#-advanced-python-features)
* [How to Run](#-how-to-run)

---

## Project Overview

The **Sentiment Service Bot** simulates a real-world customer service environment.

The system:

* Communicates with users through an AI-powered conversational interface.
* Maintains contextual memory throughout the conversation.
* Stores conversation history for later analysis.
* Evaluates the sentiment of user and bot messages.
* Generates visual analytics to assess the quality and tone of the interaction.
* Identifies potential pain points and sources of user frustration.

The project combines conversational AI with data analysis to provide insights into customer interactions.

---

## Key Features

### Intelligent Conversational Engine

* **`ServiceManager` Class:**
  Central OOP component responsible for managing the bot lifecycle, conversation flow, and analysis process.

* **Gemini API Integration:**
  Integrates Google's Gemini Large Language Model to provide dynamic, context-aware responses.

* **Custom System Prompt:**
  Defines the bot's professional customer service persona and response behavior.

* **Contextual Memory:**
  Maintains the conversation history using a structured list of dictionaries, allowing the AI to preserve context throughout the session.

---

## Technical Architecture

The project is structured around several core components:

### 1. Conversational Layer

Responsible for:

* User interaction.
* Communication with the Gemini API.
* Maintaining conversation context.
* Managing the customer service workflow.

### 2. Data Persistence Layer

Responsible for:

* Saving conversation histories.
* Loading previous conversation logs.
* Preparing stored data for analysis.

### 3. Sentiment Analysis Engine

Responsible for:

* Cleaning and normalizing text.
* Identifying positive and negative keywords.
* Calculating sentiment scores.
* Processing conversation data for statistical analysis.

### 4. Visualization Layer

Responsible for transforming sentiment data into visual charts that provide insights into the customer interaction.

---

## Data Persistence

Conversation data is persisted using **JSON serialization**.

### JSON Storage

At the end of each session, the conversation history is exported to a structured JSON file.

### Dynamic Loading

The project includes functionality for loading previously saved JSON logs for historical analysis and post-processing.

### Exception Handling

The application uses `try-except` blocks to handle potential errors, including:

* API connectivity issues.
* Missing JSON files.
* File I/O errors.
* File permission problems.

---

## Sentiment Analysis

The project includes a custom sentiment analysis engine designed to evaluate the emotional tone of conversations.

### Text Normalization

User messages are processed using string manipulation techniques to:

* Clean the input text.
* Remove punctuation.
* Normalize the text.
* Prepare messages for sentiment scoring.

### Custom Sentiment Dictionary

A domain-specific dictionary maps positive and negative keywords to sentiment values.

Each message receives an emotional score based on the detected keywords.

### Efficient Text Processing

The implementation uses:

* List comprehensions.
* Dictionary comprehensions.
* Iterators and generators.

These techniques allow the conversation data to be processed efficiently.

---

## Data Visualization

The project uses **Matplotlib** to transform conversation data into visual insights.

### Sentiment Trend

A line chart tracks cumulative sentiment throughout the conversation.

An upward trend can indicate an improvement in the user's emotional state during the interaction.

### Tone Comparison

A bar chart compares the average sentiment scores of the **user** and the **bot**, providing an overview of the tone maintained throughout the conversation.

### Pain Point Analysis

A bar chart displays the frequency of detected negative keywords, helping identify common sources of user frustration.

---

## Advanced Python Features

The project demonstrates practical use of several Python programming concepts:

* **Object-Oriented Programming (OOP)**
* **Generators and Iterators**
* **List Comprehensions**
* **Dictionary Comprehensions**
* **String Processing**
* **JSON Serialization**
* **Exception Handling**
* **API Integration**
* **Data Analysis**
* **Data Visualization with Matplotlib**

### Generators and Iterators

Generators are used to traverse conversation history efficiently while avoiding unnecessary memory usage.

### Comprehensions

List and dictionary comprehensions are used extensively for filtering conversation data and calculating sentiment scores.

### String Processing

Built-in Python string operations are used for text cleaning, normalization, and formatting before sentiment analysis.

---

## How to Run

### 1. Open the Notebook

Open the project notebook in either **Jupyter Notebook** or **Visual Studio Code**.

```text
recipes.ipynb
```

### 2. Configure the Gemini API Key

Make sure a valid **Google Gemini API key** is configured before running the notebook.

### 3. Run the Notebook

Run the notebook cells sequentially to initialize the service bot and start the interactive conversation.

### 4. Start the Conversation

Enter messages when prompted by the bot.

To end the conversation, type:

```text
exit
```

or:

```text
quit
```

### 5. Review the Results

After the conversation ends, the project generates:

* A JSON file containing the conversation history.
* Sentiment analysis results.
* Analytical charts visualizing the interaction.

---

## Project Highlights

This project demonstrates practical experience with:

* AI and LLM API integration
* Object-Oriented Python development
* Conversational application design
* Context management and data persistence
* Sentiment analysis
* Text processing
* Data analysis
* Data visualization
* Exception handling
* Efficient Python programming techniques
