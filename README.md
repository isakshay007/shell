
# NL2Shell 👨‍💻

## Overview
The **NL2Shell** application is a Streamlit-based tool powered by **Lyzr Agent API**. It translates natural language inputs into precise shell commands, simplifying command-line operations for users of all skill levels. By leveraging advanced AI capabilities, this app provides accurate and actionable shell commands based on user input.

---

## Features
- **AI-Driven Shell Command Generator**:
  - Analyze natural language inputs to generate accurate shell commands.
  - Provides clear explanations for the generated commands.
- **Tool Integration**:
  - Utilizes `perplexity_search` for enhanced context-aware command generation.
- **Interactive UI**:
  - User-friendly interface for entering natural language queries.
  - Displays the corresponding shell commands with explanations.

---

## Installation

### Prerequisites
- **Python**: Ensure Python 3.8 or higher is installed.
- **Dependencies**: Install required packages via `requirements.txt`.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/nl2shell.git
   cd nl2shell
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your **API Keys**:
   - Create a `.env` file in the project directory.
   - Add your API keys in the following format:
     ```env
     OPENAI_API_KEY="your_openai_api_key"
     LYZR_API_KEY="your_lyzr_api_key"
     ```

4. Run the application:
   ```bash
   streamlit run app.py
   ```

5. Open your browser and navigate to:
   ```
   http://localhost:8501
   ```

---

## Usage

1. **Enter Natural Language Query**: Input your desired shell operation in plain language.
   - Example: *"List all files in the current directory sorted by size."*

2. **Generate Shell Commands**: Click the **"Generate!"** button to view the generated shell command.

3. **Review Results**: The app provides a shell command tailored to your input, along with an explanation.

---

## File Structure
```
nl2shell/
│
├── app.py                  # Main application file
├── lyzr_agent.py           # Lyzr Agent API integration
├── requirements.txt        # Python dependencies
├── .env                    # API key configuration
└── .streamlit/             # Streamlit configuration
    └── config.toml         # UI settings
```

---

## Key Functionalities

### 1. **Natural Language Input**
- Accepts plain language descriptions of shell tasks or operations.

### 2. **Shell Command Generation**
- Uses Lyzr Agent API and OpenAI models to generate accurate shell commands.

### 3. **Explanations**
- Provides detailed explanations for the generated shell commands.

---

## Dependencies

- **Streamlit**: Interactive UI framework.
- **Lyzr Agent API**: Integrates advanced AI capabilities.
- **dotenv**: Manages environment variables securely.
- **requests**: Handles API interactions.
- **Python (>=3.8)**

### Install all dependencies with:
```bash
pip install -r requirements.txt
```

---

## Acknowledgments
- Built with the **Lyzr Agent API**.
- Designed to simplify command-line tasks and enhance productivity.
