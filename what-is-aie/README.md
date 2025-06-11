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
git clone https://github.com/your-username/ai-engineering-unpacked.git

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

#### 6. Verify Setup

Make sure you are in `what-is-aie` directory, then test your setup by running a quick check:

```bash
python -c "from dotenv import load_dotenv; import os; load_dotenv(); print('✅ Setup successful!' if os.getenv('GEMINI_API_KEY') else '❌ API key not found')"
```

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
   - Or run all cells using `Cell > Run All` from the menu

#### Alternatively, you can use VS Code

### What You'll Learn

As you work through the notebook, you'll see:
- How to connect to Google Gemini API
- Simple Q&A functionality with LLMs
- Query routing and specialization
- Interactive chatbot implementation
- Best practices for prompt engineering

## Code Structure

### Part 1: Simple Q&A
- `simple_ai_coach(question)`: Basic question answering
- Demonstrates direct API usage with educational context

### Part 2: Query Routing
- `route_query(question)`: Analyzes questions and determines appropriate specialist
- Should return one of: `AI_CONCEPTS`, `PYTHON_CODING`, `CAREER_GUIDANCE`, `GENERAL`

### Part 3: Specialized Coaches
- `ai_concepts_coach(question)`: Handles AI/ML theory questions
- `python_coding_coach(question)`: Handles programming questions
- `career_guidance_coach(question)`: Handles career-related questions
- `general_coach(question)`: Handles other questions

### Part 4: Smart Routing
- `smart_ai_coach(question)`: Main function that combines routing with specialists
- Returns both the routing decision and the specialist's response

### Part 5: Interactive Mode
- `interactive_coach()`: Command-line interface for testing
- Perfect for Jupyter notebook cells

## Customization

You can easily extend this system by:

1. **Adjusting Prompts**: For better results and experience
2. **Adding New Specialists**: Create new coach functions with specialized prompts and add new categories for routing

## Troubleshooting

- **API Key Issues**: Ensure your `.env` file is in the correct directory
- **Import Errors**: Make sure all dependencies are installed
