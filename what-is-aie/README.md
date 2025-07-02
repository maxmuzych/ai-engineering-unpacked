# AI Learning Coach Chatbot

A simple example demonstrating how to use LLMs through API. Created for ["What is AI Engineering?"](https://www.aiunpacked.net/p/what-is-ai-engineering) issue.
This chatbot helps answer questions about AI concepts, Python coding, and career guidance.

## Features

- **Simple Q&A**: Basic question-answering functionality
- **Smart Routing**: Automatically routes queries to specialized "coaches"
- **Three Specialists**:
  - 🧠 **AI Concepts Coach**: Machine learning, neural networks, algorithms
  - 🐍 **Python Coding Coach**: Syntax, libraries, best practices
  - 💼 **Career Guidance Coach**: Skills, learning paths, job market

## Getting Started

**📖 For complete setup instructions, see the [Project Setup Guide](../SETUP.md)**

Quick overview:
1. Clone the repository and set up Python environment
2. Install dependencies: `pip install -r what-is-aie/requirements.txt`
3. Get your [Gemini API key](https://aistudio.google.com/) and add to `.env` file
4. Run the Jupyter notebook

## Usage

### Running the Jupyter Notebook

1. **Start Jupyter Notebook**:
   ```bash
   # Make sure you're in the what-is-aie directory
   cd what-is-aie
   
   # Start Jupyter Notebook
   jupyter notebook
   ```

2. **Open the AI Learning Coach Notebook**:
   - Your browser will open automatically
   - Open the `ai_learning_coach.ipynb` notebook

3. **Run the Notebook**:
   - Execute cells one by one using `Shift + Enter`


### What You'll Learn

As you work through the notebook, you'll see:
- How to connect to Google Gemini API
- Simple Q&A functionality with LLMs
- Query routing and specialization
- Interactive chatbot implementation
- Best practices for prompt engineering
