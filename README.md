# Text_to_SQL AI Agent 🤖💻

## Overview ✨
Text_to_SQL AI Agent is a Streamlit-based application that converts natural language queries into SQL commands and retrieves relevant data from an SQLite database.

## Features 📝
- 🔎 **Natural Language Processing**: Converts English questions into SQL queries.
- 💻 **Database Interaction**: Fetches data from an SQLite database based on generated SQL queries.
- 🛠️ **Easy to Use**: Simple UI with Streamlit for seamless user experience.

## Technologies Used ⚙️
- Python
- Streamlit
- SQLite
- Langchain
- GROQ LLM (Llama3-8b-8192)

## Installation ⚖️
### Prerequisites
Ensure you have Python installed on your system.

1. Clone this repository:
   ```sh
   git clone https://github.com/your-repo/Text_to_SQL.git
   cd Text_to_SQL
   ```

2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

3. Set up the environment variable:
   ```sh
   export GROQ_API_KEY='your_groq_api_key'
   ```

## How to Use ✨
1. Run the application:
   ```sh
   streamlit run app.py
   ```
2. Enter your query in natural language (e.g., *How many students are in the Data Science course?*).
3. View the SQL query generated and the corresponding results from the database.

## Code Overview 📚
### Main Application (`app.py`)
- Uses **Streamlit** for UI.
- Takes user input and converts it into an SQL query using **Langchain** and **GROQ LLM**.
- Executes the SQL query on an SQLite database and displays results.

### Database Setup (`setup_db.py`)
- Creates an SQLite database `student.db`.
- Defines a `STUDENT` table with fields: `NAME`, `COURSE`, `SECTION`, `MARKS`.
- Inserts sample data.

## Example Queries 📋
| Natural Language Query | SQL Query |
|------------------------|-----------|
| How many students are there? | `SELECT COUNT(*) FROM STUDENT;` |
| Show all students in Data Science. | `SELECT * FROM STUDENT WHERE COURSE='Data Science';` |

## Contributing 👥
Contributions are welcome! Feel free to fork, modify, and submit pull requests.

## License ©
This project is licensed under the Apache License.

---
🛠️ Built with passion for database interaction and AI-driven solutions!

