# Population and Notes Query Agent

This project is a multi-functional query agent powered by Python and the `llama_index` library. It provides detailed insights into world population statistics, demographics, and country-specific data (e.g., Canada). Additionally, it enables users to save notes directly into a file.

---

## Features

1. **World Population Analysis**:
   - Query population and demographic data using a CSV file.
   - Execute Python code dynamically to process data using Pandas.

2. **Canada Country Data**:
   - Load and query detailed information from a PDF file about Canada using vector-based search.

3. **Note-Saving Tool**:
   - Save textual notes into a local file (`notes.txt`) using a dedicated tool.

4. **Interactive User Input**:
   - Accepts prompts from users in a command-line interface.
   - Provides detailed and contextual responses based on the user's query.

---

## Components

### 1. **`main.py`**
- This script is the entry point of the application.
- It loads population data, initializes tools, and creates a query agent.
- Prompts are taken from the user in an interactive loop.

### 2. **`note.py`**
- Defines a tool to save notes into a file.
- Uses the `llama_index` library's `FunctionTool` to create a function-based tool for note-saving.

### 3. **`pdf.py`**
- Reads and indexes a PDF file (`Canada.pdf`) for querying.
- Utilizes vector-based storage for efficient retrieval.

### 4. **`prompts.py`**
- Contains custom prompt templates and instructions for processing Pandas queries.

---

## Prerequisites

- **Python 3.7+**
- Install the required dependencies using:

  ```bash
  pip install pandas llama-index python-dotenv
  ```
### File Structure
```
  project-root/
├── data/
│   ├── population.csv
│   ├── Canada.pdf
├── main.py
├── note.py
├── pdf.py
├── prompts.py
├── .env
├── README.md
└── requirements.txt
```



