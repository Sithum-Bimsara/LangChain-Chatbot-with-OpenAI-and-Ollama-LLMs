# Langchain Chatbot with OpenAI and Ollama LLMs

This project demonstrates a simple chatbot powered by two LLMs: OpenAI's GPT-3.5 and Ollama's Llama3.2. The project includes two separate scripts:
- `app.py`: A Streamlit application using OpenAI's LLM.
- `localama.py`: A Streamlit application using Ollama's Llama3.2 LLM.

## What is Streamlit?

Streamlit is an open-source app framework used to build interactive web applications with Python. It's particularly useful for creating data applications and machine learning demos, allowing developers to quickly prototype and deploy apps.

## What is Ollama?

Ollama provides access to large language models (LLMs) like Llama3.2. It allows you to run models on your local machine, offering an easy-to-use platform to interact with AI-powered models.

## Prerequisites

Before you begin, make sure you have the following installed:
- Python 3.7 or higher
- pip (Python package installer)
- Ollama (For Llama3.2 model)

To install Ollama, follow these steps:
1. Go to [Ollama's website](https://ollama.com/).
2. Download and install Ollama based on your OS.
3. After installation, run the following command to download the Llama3.2 model:

```bash
ollama run llama3.2
```

This will pull and install the model locally on your machine.

## Project Structure

chatbot/
│
├── app.py                 # Streamlit app using OpenAI LLM
├── localama.py            # Streamlit app using Llama3.2 LLM
.env                       # Environment variables for API keys
requirements.txt           # List of dependencies
venv/                      # Virtual environment (optional, created manually)
README.md                  # Project documentation

## Setup Instructions

# 1. Clone the repository
First, clone this repository to your local machine:
```
git clone https://github.com/Sithum-Bimsara/LangChain-Chatbot-with-OpenAI-and-Ollama-LLMs.git
cd LangChain-Chatbot-with-OpenAI-and-Ollama-LLMs
```

# 2. Create a Virtual Environment
If you haven't already created a virtual environment (venv), follow these steps to set it up:

On Windows:
```
python -m venv venv
```

On macOS/Linux:
```
python3 -m venv venv
````

# 3. Activate the Virtual Environment
On Windows:
```
.\venv\Scripts\activate
```
On macOS/Linux:
```
source venv/bin/activate
```

# 4. Install Dependencies
Once the virtual environment is activated, install the required dependencies from requirements.txt:
```
pip install -r requirements.txt
```

# 5. Set Up Environment Variables
Create a .env file in the root directory (if it doesn't exist) and add the following environment variables for your API keys:
```
LANGCHAIN_API_KEY="your_langchain_api_key"
OPENAI_API_KEY="your_openai_api_key"
LANGCHAIN_PROJECT="Tutorial1"
```
Make sure to replace `"your_langchain_api_key"` and `"your_openai_api_key"` with your actual API keys.

# 6. Run the Application
To run the OpenAI-powered chatbot `(app.py`:
```
streamlit run app.py
```
To run the Ollama-powered chatbot `(localama.py)`:
```
streamlit run localama.py
```
Once the app is running, it will be accessible in your browser at `http://localhost:8501`.

# 7. Stopping the App
To stop the application, simply press `Ctrl+C` in the terminal where the app is running.

## Requirements
The dependencies for this project are listed in `requirements.txt`. You can view the contents of requirements.txt below:
```
streamlit>=1.24.0
python-dotenv>=1.0.0
openai>=0.27.4
langchain-core>=0.0.1
langchain-community>=0.0.1
langchain-ollama>=0.0.1
```
## Troubleshooting
Ensure that your `.env` file contains valid API keys and there are no syntax issues.
If you encounter errors related to missing packages, try running pip install -r requirements.txt again.
Make sure you're using a Python version of 3.7 or higher.
If you haven't downloaded the Llama3.2 model using Ollama, run the command `ollama run llama3.2`.

## Contributing
Feel free to fork this repository and submit pull requests if you'd like to contribute to the project.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

