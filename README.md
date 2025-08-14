# 🐦🐦 SQL Chatbot using LangChain & Streamlit 🐦🐦

🚀 A smart, conversational chatbot that lets you interact with your SQL database *using plain English* 
 — no SQL knowledge required!  
Built with *LangChain* for natural language processing, *Streamlit* for a sleek interface, and your favorite database as the backend.  

💡 Just ask a question like "Show me the top 5 customers by sales" and watch it instantly turn into SQL, execute it, and give you the results.

## 📸 Demo

Here’s a quick look at the SQL Chatbot in action:

![SQL Chatbot Demo](assets/demo.gif)
add video 

![SQL Chatbot Screenshot](assets/screenshot.png)
add screenshot

## 🤖 What Does the SQL Chatbot Do?

This chatbot bridges the gap between *natural language* and *SQL queries*.  
You don’t have to remember any SQL commands — just type your question in plain English.

### 🔍 How It Works for You:
- *Ask in English* → "Show me sales in January 2024"
- *Chatbot Converts* → Generates the exact SQL statement
- *Executes & Fetches* → Runs the query on your database
- *Shows Results* → Displays data in a clean, interactive table
- *Download Option* → Export your results instantly as a CSV

✨ Think of it as your personal database assistant — always ready to answer, 24/7.

## 🌟 Features

✅ *Natural Language to SQL* – No need to write SQL manually, just ask in plain English.  
✅ *Supports Multiple Databases* – Works with SQLite, MySQL, or PostgreSQL.  
✅ *Instant Execution* – Query runs in real time with fast results.  
✅ *CSV Export* – Download your results in one click. (Ongoing) </br>
✅ *Simple UI* – Built with Streamlit for a clean and minimal experience.  
✅ *Beginner-Friendly* – Perfect for those new to SQL.


## 🔄 How It Works – Flowchart

mermaid
flowchart TD
    A[📝 User Types a Question in English] --> B[🤖 LangChain Processes the Query]
    B --> C[📜 LLM Generates SQL Statement]
    C --> D[🗄 SQL Query Runs on Database]
    D --> E[📊 Results Fetched using Pandas]
    E --> F[💻 Displayed in Streamlit App]
    F --> G[⬇ Optional: Download Results as CSV]


## 🛠 Tech Stack

*Languages & Frameworks*
- 🐍 Python
- 🖥 Streamlit – For the interactive web app
- 🤖 LangChain – Natural language to SQL conversion
- 🗄 SQLite / MySQL / PostgreSQL – Database backend
- 🐼 Pandas – Data handling & formatting

*APIs & Services*
- OpenAI API (or your chosen LLM provider)

*Version Control*
- Git & GitHub

## ⚙ Installation & Using

1️⃣ *Clone the repository*
bash
git clone https://github.com/yourusername/sql-chatbot.git
cd sql-chatbot

2️⃣*Create a virtual environment*
bash
python -m venv venv
venv\Scripts\activate 

3️⃣*Install dependencies*
bash
pip install -r reqq.txt

4️⃣*Run the app*
bash
streamlit run app.py


## 🔧 How to use

1️⃣ Fronm left sidebar choose between </br>
- SQLLite </br>
- MYSQL </br>

2️⃣ If SQLLite </br>
- Input your GROQ LLM key </br>
  (Note this code is hard coded for GROQ only) </br>
  (I will be using multiple LLMs in Future Improvements) </br>

3️⃣ If MYSQL </br>
Configure your database connection </br>

python
MySQL Hostname = "Enter your host name"
MySQL Username = "Enter your username"
MySQL Password = "Enter your password"
MySQL Database Name = "Enter your database name"
Groq API Key = "Enter your Groq Api Key"


## Ask your question
chat
"Show me the top 5 products by sales in 2024"

 - Get your results instantly

## 📂 Project Structure

sql-chatbot/ </br>
│-- app.py               # Main Streamlit application </br>
│-- config.py            # Database configuration settings </br>
│-- requirements.txt     # Python dependencies </br>
│-- .env.example         # Example environment variables </br>
│-- README.md            # Project documentation </br>
│-- assets/              # Screenshots, GIFs, diagrams </br>
│     ├── demo.gif </br>
│     ├── screenshot.png </br>
│     └── flowchart.png </br>

## 🚀 Future Improvements

- 🔄 *Multi-LLM Support* – Compare results from different LLMs (using LangGraph).
- 📊 *Advanced Analytics* – Support for more complex analytical SQL queries.
- 🔐 *User Authentication* – Secure access with login for private databases.
- 🌐 *Cloud Deployment* – Host on platforms like Streamlit Cloud, AWS, or Hugging Face Spaces.
- 🗣 *Voice Input* – Ask database queries using speech-to-text.
- 📅 *Scheduled Reports* – Automatically email query results at set intervals.


## 📜 License

This project is licensed under the *MIT License* — you’re free to use, modify, and distribute it, provided you include the original license notice.

See the [LICENSE](LICENSE) file for full details.
