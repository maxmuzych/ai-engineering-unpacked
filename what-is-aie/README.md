# AI Learning Coach Chatbot

A simple example demonstrating how to use LLMs through API for educational purposes. This chatbot helps answer questions about AI concepts, Python coding, and career guidance.

## Features

- **Simple Q&A**: Basic question-answering functionality
- **Smart Routing**: Automatically routes queries to specialized "coaches"
- **Three Specialists**:
  - 🧠 **AI Concepts Coach**: Machine learning, neural networks, algorithms
  - 🐍 **Python Coding Coach**: Syntax, libraries, best practices
  - 💼 **Career Guidance Coach**: Skills, learning paths, job market

## Getting Started

### Prerequisites

Before you begin, make sure you have:
- [Python](https://www.python.org/downloads/) 3.8 or higher installed
- [Git](https://git-scm.com/downloads) installed on your system
- A [Google account](https://accounts.google.com/) to access Google AI Studio

### Step-by-Step Setup

#### 1. Clone the Project

```bash
# Clone the repository
git clone https://github.com/maxmuzych/ai-engineering-unpacked.git

# Navigate to the project directory
cd ai-engineering-unpacked
```

#### 2. Set Up Python Environment (Recommended)

Create a virtual environment to keep dependencies isolated:

```bash
# Create virtual environment
python -m venv .venv

# Activate virtual environment
# On macOS/Linux:
source .venv/bin/activate
# On Windows:
.venv\Scripts\activate
```

#### 3. Install Dependencies

```bash
# Install required packages
pip install -r what-is-aie/requirements.txt
```

#### 4. Get Your Gemini API Key

1. Visit [Google AI Studio](https://aistudio.google.com/)
2. Sign in with your Google account
3. Click "Get API Key" in the top navigation
4. Create a new API key or use an existing one
5. Copy the API key (keep it secure!)

#### 5. Set Up Environment Variables

Create a `.env` file in the `what-is-aie` directory:

Add your API key to the `.env` file:
```
GEMINI_API_KEY=your_api_key_here
```

**Important**: Never commit your `.env` file to version control. It's already included in `.gitignore`.

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

#### Alternatively, you can use VS Code

### What You'll Learn

As you work through the notebook, you'll see:
- How to connect to Google Gemini API
- Simple Q&A functionality with LLMs
- Query routing and specialization
- Interactive chatbot implementation
- Best practices for prompt engineering