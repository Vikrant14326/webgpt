WebGPT Chatbot with Internet Search Capabilities
This project is a Streamlit-based WebGPT chatbot that integrates OpenAI's GPT models with internet search capabilities powered by DuckDuckGo. The chatbot can perform conversational tasks, respond intelligently using GPT models, and fetch real-time information from the web when necessary.

Features
Interactive Chat Interface: User-friendly chat interface built using Streamlit.
Multiple GPT Models: Supports both GPT-3.5 and GPT-4 for responses.
Web Search Integration: Leverages DuckDuckGo to fetch search results, PDFs, videos, images, and news.
Function Calling: Implements function calling to handle web search responses dynamically.
Session Management: Maintains chat history and conversation context.
Installation
Prerequisites
Python 3.9 or above.
Required dependencies (listed in requirements.txt).
Steps
Clone the repository:

bash
Copy code
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
Create a virtual environment and activate it:

bash
Copy code
python -m venv venv
source venv/bin/activate # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Streamlit application:

bash
Copy code
streamlit run webgpt_app.py
Project Structure
graphql
Copy code
<repo-name>/
├── requirements.txt       # Dependencies for the project
├── webgpt_app.py          # Main Streamlit application
├── web_search.py          # Module for DuckDuckGo search functions
└── utils/
    ├── load_config.py     # Configuration loader (not provided in files)
    ├── app_utils.py       # Utility functions for the app (not provided in files)
    └── ...                # Other helper modules
How It Works
Chat Interface:

Users can interact via a chat box.
Responses are generated based on user input.
Web Search Integration:

If GPT requires external information, a web search is triggered.
DuckDuckGo APIs fetch results for various media types (text, PDFs, images, etc.).
GPT Models:

Uses OpenAI's GPT-3.5 or GPT-4 based on user preference.
Chat history and context are preserved across interactions.
Usage
Start the app using the Streamlit command provided above.
Use the sidebar to:
Select the GPT model.
Reset the conversation.
Interact with the chatbot by typing queries in the chat box.
If necessary, the chatbot will fetch real-time information using web search.
Dependencies
All required libraries are listed in requirements.txt. Key dependencies include:

streamlit: For building the web application.
openai: For accessing GPT models.
duckduckgo_search: For performing web searches.
python-dotenv: For managing environment variables.
Future Enhancements
Add support for additional search providers.
Improve error handling for function calls.
Extend functionality to fetch structured data like JSON APIs.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
OpenAI for GPT models.
DuckDuckGo for search API.
The Streamlit community for the interactive app framework.
