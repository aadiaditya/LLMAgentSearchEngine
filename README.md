# LangChain - Chat with Search

This Streamlit application integrates LangChain to provide a chatbot that can search the web and retrieve information from various sources, including Arxiv, Wikipedia, and DuckDuckGo.

## Features

- **Interactive Chatbot**: Engage with a chatbot that can answer questions by searching the web.
- **Search Tools**: Uses Arxiv, Wikipedia, and DuckDuckGo for information retrieval.
- **Streamlit UI**: An intuitive user interface built with Streamlit.
- **Real-time Feedback**: See the agent's thoughts and actions in real-time.

## Setup

### Prerequisites

- Python 3.7 or later
- Streamlit
- LangChain

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-repo/langchain-chat-search.git
    cd langchain-chat-search
    ```

2. **Create a virtual environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:
    Create a `.env` file in the root directory and add your Groq API key:
    ```env
    GROQ_API_KEY=your_groq_api_key
    ```

### Running the App

1. **Start the Streamlit app**:
    ```bash
    streamlit run app.py
    ```

2. **Interact with the chatbot**:
    - Open the app in your browser (usually at `http://localhost:8501`).
    - Enter your Groq API key in the sidebar.
    - Start chatting with the bot by entering prompts in the chat input.

## Code Overview

### app.py

This is the main file that sets up the Streamlit app and the LangChain agents.

- **Imports**: Necessary libraries and tools from LangChain and Streamlit.
- **Initialize Tools**: Set up the Arxiv, Wikipedia, and DuckDuckGo search tools.
- **Streamlit UI**: Define the main title, sidebar for settings, and chat interface.
- **Chat Logic**: Handles user input, initializes the LangChain agent, and displays the chatbot responses.

### Dependencies

- **Streamlit**: For the web interface.
- **LangChain**: For the language model and agent setup.
- **dotenv**: For loading environment variables from the `.env` file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [LangChain](https://github.com/langchain-ai/langchain)
- [Streamlit](https://streamlit.io/)
- [Groq](https://groq.com/)
