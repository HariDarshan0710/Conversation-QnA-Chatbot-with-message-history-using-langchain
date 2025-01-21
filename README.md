# Conversation-QnA-Chatbot-with-message-history-using-langchain
Conversation QnA Chatbot with message history using langchain

### Conversation Q&A Chatbot
In many Q&A applications we want to allow the user to have a back-and-forth conversation, meaning the application needs some sort of "memory" of past questions and answers, and some logic for incorporating those into its current thinking.

- Chains, in which we always execute a retrieval step;
- Agents, in which we give an LLM discretion over whether and how to execute a retrieval step (or multiple steps).

# Conversation-QnA-Chatbot-with-message-history-using-langchain

## Overview

This project showcases a **Conversational Q&A Chatbot** built using **LangChain**, capable of maintaining **message history** to provide context-aware responses. The chatbot leverages advanced natural language processing techniques to understand user queries, track conversational history, and deliver accurate and relevant answers.

## Features

- **Context-aware conversations**: Retains message history for better understanding of queries in context.
- **Question-answering capabilities**: Answers questions based on embedded knowledge or external sources.
- **Extensibility**: Easily integrates with various backends and APIs.
- **Modular design**: Customizable components for specialized use cases.

## Technologies Used

- **LangChain**: Framework for building applications powered by large language models (LLMs).
- **Python**: Programming language for implementation.
- **Streamlit**: For creating a user-friendly chatbot interface (optional).
- **OpenAI API**: For leveraging LLMs (like GPT models).
- **Memory Management**: LangChain’s built-in memory modules for retaining conversation history.

## Setup and Installation

### Prerequisites

Ensure you have the following installed on your system:

- Python 3.8 or higher
- pip (Python package installer)
- OpenAI, Groq API key

### Installation Steps

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/Conversation-QnA-Chatbot-with-message-history-using-langchain.git
   cd Conversation-QnA-Chatbot-with-message-history-using-langchain
   ```

2. **Create a virtual environment** (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   Create a `.env` file in the project directory with your OpenAI API key:

   ```env
   OPENAI_API_KEY=your_openai_api_key
   ```

5. **Run the chatbot**:

   ```bash
   python app.py
   ```

   If using Streamlit for the interface:

   ```bash
   streamlit run app.py
   ```

## Usage

1. Open the chatbot interface (e.g., Streamlit app) in your browser.
2. Start a conversation by typing your queries.
3. The chatbot will respond, keeping track of the conversational context.

## Directory Structure

```
Conversation-QnA-Chatbot-with-message-history-using-langchain/
|-- app.py                 # Main application script
|-- requirements.txt       # Python dependencies
|-- .env                   # Environment variables
|-- README.md              # Project documentation
|-- utils/
    |-- memory.py          # Memory management functions
    |-- langchain_utils.py # LangChain configuration and utilities
```

## Key Components

- **LangChain Memory**: Tracks message history for context-aware conversations.
- **LLM Integration**: Powered by Open source Groq API for robust Q&A capabilities.
- **Frontend Interface**: Optional Streamlit-based UI for enhanced user interaction.

## Customization

### Adding New Features

1. **Modify the prompt engineering**: Update the conversation logic in the `langchain_utils.py` file.
2. **Integrate external data sources**: Use LangChain’s document loaders to fetch data from knowledge bases or APIs.
3. **Enhance memory management**: Implement custom memory logic in `memory.py` to suit your needs.

### Changing LLMs

Replace the OpenAI API configuration with other LLM providers like Anthropic, Hugging Face, or Azure OpenAI by updating `langchain_utils.py`.

## Example Conversation

**User**: What is LangChain?

**Chatbot**: LangChain is a framework for developing applications powered by large language models (LLMs) with a focus on composability and modularity.

**User**: Can you explain how it works?

**Chatbot**: Sure! LangChain provides tools to chain together LLMs with prompts, memory, and external data sources to create dynamic and context-aware applications.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a pull request with a detailed description of your updates.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The LangChain team for their powerful framework.
- OpenAI for providing cutting-edge Groq APIs.

