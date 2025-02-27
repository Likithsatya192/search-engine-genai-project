# LangChain Search Chatbot


This project is a **Streamlit-based chatbot** that utilizes **LangChain** and **Groq API** to answer user queries by searching the web using **DuckDuckGo, Wikipedia, and Arxiv**. It integrates **LLM (Large Language Models)** to generate intelligent responses.


## Features
- ✅ Interactive chatbot with **Streamlit UI**
- 🔎 Searches the web using **DuckDuckGo, Wikipedia, and Arxiv**
- 🤖 Uses **Groq API (Llama3-8b-8192 model)** for generating responses
- ⚡ Supports real-time streaming responses
- 🗂 Maintains chat history using `st.session_state`


## Environment Variables
Create a `.ven` file in the project directory and add:
```
GROQ_API_KEY=your_api_key_here
```


Alternatively, enter your API key in the Streamlit sidebar.


## Usage
Run the chatbot with:
```bash
streamlit run app.py
```


## Project Structure
```
📂 langchain-search-chatbot/
│-- app.py  # Main Streamlit app
│-- requirements.txt  # Required dependencies
│-- .ven  # API Key storage
│-- README.md  # Documentation
```


## Explanation of Core Components
- **`st.session_state`** → Stores chat history
- **`ChatGroq`** → Uses Groq API for LLM processing
- **`DuckDuckGoSearchRun`** → Fetches live search results
- **`WikipediaQueryRun` & `ArxivQueryRun`** → Retrieves data from Wikipedia and Arxiv
- **`initialize_agent`** → Combines LLM and tools for intelligent query processing
- **`st.chat_message` & `st.chat_input`** → Handles Streamlit chat UI


## Known Issues
- Ensure you have a **valid API key** before running the app
- Some searches may take longer depending on external API response times


## Author
👨‍💻 Developed by **Likith Sagar**


---
🌟 **Enjoy building with LangChain!** 🌟

