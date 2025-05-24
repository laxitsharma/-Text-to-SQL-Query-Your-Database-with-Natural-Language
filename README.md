# -Text-to-SQL-Query-Your-Database-with-Natural-Language
This project is a simple but powerful Streamlit web application that allows users to interact with a SQLite database using natural language. Leveraging LangChain, Groq LLM (LLaMA3-8B), and LangChain's SQL prompt engineering, this app automatically converts English questions into valid SQL queries, executes them, and displays the results.

🔧 Features
✅ Translate plain English into SQL queries

✅ Query a preloaded STUDENT database (columns: NAME, COURSE, SECTION, MARKS)

✅ Powered by LangChain and Groq LLM

✅ Interactive and user-friendly Streamlit interface

✅ Works locally with SQLite backend

📋 Example Questions You Can Ask
"What are the average marks class wise?"

"Name of the student who scored the highest marks?"

"Who has the second highest marks in the DEVOPS course?"

🚀 Getting Started
1. Install dependencies
bash
Copy
Edit
pipenv install streamlit langchain_groq
2. Set your Groq API Key
Set the environment variable:

bash
Copy
Edit
export GROQ_API_KEY=your_key_here
3. Run the app
bash
Copy
Edit
streamlit run app.py
🗂 Files Overview
app.py – Streamlit UI + LLM SQL conversion logic

database.py – Initializes the SQLite database with sample student data

student.db – The database file automatically generated on first run

readme.md – Project info and example prompts

📌 Notes
No SQL knowledge needed – just type your question!

The SQL generated does not include unnecessary formatting or markdown, ensuring direct execution.


