# Gemini Service Chatbot & Analytics

An intelligent customer service chatbot powered by the Gemini API, featuring contextual memory management, real-time sentiment analysis, and automated service quality visualization.

## Key Features

* **Context-Aware Conversational AI**: Integrates with the Gemini API to handle complex user queries with multi-turn conversation memory.
* **Service Management**: Session and conversation state handling implemented through a centralized `ServiceManager`.
* **Sentiment Analysis Engine**: Independent analysis module that evaluates customer satisfaction and interaction quality in real time.
* **Visual Analytics**: Generates service quality reports and sentiment trends using Matplotlib.

## Architecture & Structure

```text
├── src/
│   ├── service_manager.py     # Session context, state management, and Gemini API logic
│   ├── sentiment_engine.py    # Standalone sentiment analysis and scoring algorithm
│   ├── analytics_visualizer.py # Matplotlib visualization generators
│   └── main.py                # Main application loop and entry point
├── requirements.txt           # Project dependencies
└── README.md                  # Documentation
