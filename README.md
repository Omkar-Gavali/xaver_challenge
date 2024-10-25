# xaver_challenge
Developing a RAG chatbot using Langchain  as part of a coding challenge

## Environment Setup

Before you start, you need to have Python installed.  

1. Create a virtual environment:

bash
python -m venv env


2. Activate the virtual environment:

On Windows, run:

bash
.\env\Scripts\activate

On Unix or MacOS, run:

bash
source env/bin/activate


3. Install the requirements:

bash
pip install -r requirements.txt


The `requirements.txt`  contains the necessary libraries for this project.

## API Key Setup

You need to have a Groq API key to acess the llm. 

1. Sign up or log in to Groq.
2. Go to your dashboard and generate a new API key.

bash
os.environ["GROQ_API_KEY"] = getpass.getpass()


![API Image](API.png)



Replace `your_api_key` with the actual API key you got from Groq.

## Usage

The main function to call is `chat_with_llm(prompt, chat_history=[], custom_template=PROMPT_TEMPLATE)`. 

A typical usage might look like this:

python
chat_history = []
prompt = "What's the weather like today?"
chat_with_llm(prompt, chat_history)
plaintext

You can also use the interactive mode. Just call `start_interactive_chat()` and start chatting. Type 'exit' or 'quit' to end the session.

python
start_interactive_chat()
plaintext

