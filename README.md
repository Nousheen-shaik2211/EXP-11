# EXP-11
# LCEL Story Generation Chain

## Aim
To build a simple LangChain Expression Language (LCEL) chain that generates short stories from user-provided topics.

## Problem Statement
Create an LCEL chain using a prompt template, an OpenAI language model, and a string output parser. Invoke the chain with at least two different topics and print the generated stories.

## Technologies Used
- Python
- LangChain
- LangChain OpenAI
- OpenAI GPT-3.5-turbo

## Algorithm
1. Install the required packages.
2. Set the OpenAI API key as an environment variable.
3. Import `ChatPromptTemplate`, `ChatOpenAI`, and `StrOutputParser`.
4. Define a prompt template containing `{topic}`.
5. Initialize the language model.
6. Build the chain using `prompt | llm | parser`.
7. Invoke the chain with two hardcoded topics.
8. Print the generated stories.

## Project Structure
```text
LCEL_Story_Generation/
├── main.py
├── README.md
├── requirements.txt
└── .gitignore
```

## Setup and Execution

Install the dependencies:

```bash
pip install -r requirements.txt
```

Set the API key before running the script.

**Windows PowerShell:**
```powershell
$env:OPENAI_API_KEY="your_api_key_here"
python main.py
```

**Linux/macOS:**
```bash
export OPENAI_API_KEY="your_api_key_here"
python main.py
```

Replace `your_api_key_here` with your valid OpenAI API key.

## Expected Output
The program prints a short story for each topic:
- A dragon and a knight
- A lost spaceship

The actual stories are generated dynamically and may differ each time.

## Conclusion
The experiment demonstrates LCEL pipe syntax by connecting a prompt template, an LLM, and a string output parser into a single chain.
