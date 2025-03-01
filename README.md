# Agentic AI Chatbot
This project is a conversational AI chatbot built using LangChain, a framework for building conversational AI models. The chatbot is designed to interact with users through a web interface, answering their queries and providing relevant information.

## Key Features
* **LangChain Integration:** The project uses LangChain to create a conversational AI model that can understand and respond to user queries.
* **Multiple LLMs:** The project supports multiple large language models (LLMs) from different providers, including Groq and OpenAI.
* **Web Search:** The project uses Tavily for web search, allowing the chatbot to retrieve relevant information from the internet.
* **Streamlit UI:** The project uses Streamlit to create a user-friendly web interface for interacting with the chatbot.
* **FastAPI Backend:** The project uses FastAPI to create a backend API that handles requests from the frontend and interacts with the LangChain model.

## Installation
1. **Clone the repository:** 
   ```bash
   git clone https://github.com/mybarefootstory/Agentic-AI-Chatbot.git
   ```
2. **Create and activate a virtual environment:** 
   ```bash
   python -m venv venv
   venv\Scripts\activate  # On Windows
   source venv/bin/activate  # On macOS/Linux
   ```
3. **Install the required packages:** 
   ```bash
   pip install -r requirements.txt
   ```
4. **Set up your API keys:** 
   - Create a `.env` file in the project's root directory.
   - Add your API keys to the `.env` file:
     ```
     OPENAI_API_KEY=your_openai_api_key
     GROQ_API_KEY=your_groq_api_key
     TAVILY_API_KEY=your_tavily_api_key
     ```

## Usage
1. **Run the backend:** 
   ```bash
   uvicorn main:app --host 0.0.0.0 --port 9999
   ```
2. **Run the frontend:** 
   ```bash
   streamlit run front-end.py
   ```
3. **Interact with the chatbot:** Open a web browser and navigate to `http://localhost:8501`. You can then interact with the chatbot by typing queries and selecting options.

## Dependencies
The project relies on the following key libraries:
* `python-dotenv`
* `langchain_groq`
* `langchain_community`
* `langgraph`
* `pydantic`
* `fastapi`
* `uvicorn`
* `streamlit`


