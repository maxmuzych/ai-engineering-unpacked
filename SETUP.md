# Project Setup Guide

This guide covers the common setup steps for all projects in the AI Engineering Unpacked repository.

## Prerequisites

Before you begin, make sure you have:
- [Python](https://www.python.org/downloads/) 3.8 or higher installed
- [Git](https://git-scm.com/downloads) installed on your system
- A [Google account](https://accounts.google.com/) to access Google AI Studio

## Step-by-Step Setup

### 1. Clone the Project

```bash
# Clone the repository
git clone https://github.com/maxmuzych/ai-engineering-unpacked.git

# Navigate to the project directory
cd ai-engineering-unpacked
```

### 2. Set Up Python Environment (Recommended)

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

### 3. Install Dependencies

```bash
# Install required packages for specific project
# For what-is-aie:
pip install -r what-is-aie/requirements.txt

# For prompt-engineering-101:
pip install -r prompt-engineering-101/requirements.txt
```

### 4. Get Your Gemini API Key

1. Visit [Google AI Studio](https://aistudio.google.com/)
2. Sign in with your Google account
3. Click "Get API Key" in the top navigation
4. Create a new API key or use an existing one
5. Copy the API key (keep it secure!)

### 5. Set Up Environment Variables

Create a `.env` file in the specific project directory:

```bash
# For what-is-aie project:
cp what-is-aie/.env.example what-is-aie/.env

# For prompt-engineering-101 project:
cp prompt-engineering-101/.env.example prompt-engineering-101/.env
```

Add your API key to the `.env` file:
```
GEMINI_API_KEY=your_api_key_here
```

**Important**: Never commit your `.env` file to version control. It's already included in `.gitignore`.

## Running Jupyter Notebooks

### Option 1: Local Jupyter

1. **Navigate to the project directory**:
   ```bash
   # For what-is-aie:
   cd what-is-aie
   
   # For prompt-engineering-101:
   cd prompt-engineering-101
   ```

2. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

3. **Open the notebook**:
   - Your browser will open automatically
   - Select the `.ipynb` file you want to run

4. **Run the notebook**:
   - Execute cells one by one using `Shift + Enter`

### Option 2: Google Colab

You can also run notebooks in [Google Colab](https://colab.research.google.com/):
1. Upload the `.ipynb` file to Colab
2. Install dependencies in the first cell:
   ```python
   !pip install google-genai python-dotenv
   ```
3. Set up your API key in Colab's secrets or directly in the code

## Troubleshooting

### Common Issues

**Virtual Environment Not Activating**:
- Make sure you're in the correct directory
- On Windows, try `.venv\Scripts\activate.bat` instead

**API Key Not Found**:
- Ensure your `.env` file is in the correct project directory
- Check that the file contains `GEMINI_API_KEY=your_actual_key`
- Restart your Jupyter kernel after adding the API key

**Package Installation Errors**:
- Make sure your virtual environment is activated
- Try upgrading pip: `pip install --upgrade pip`
- On some systems, use `python3` and `pip3` instead

**Jupyter Not Starting**:
- Make sure Jupyter is installed: `pip install jupyter`
- Try starting with: `python -m jupyter notebook`

Need help? Check the individual project READMEs for project-specific guidance!
