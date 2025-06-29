

#  AI Assistant Chatbot

A simple AI chatbot web app powered by Flask and [Groq API](https://console.groq.com/). Users can chat with an intelligent assistant through a sleek web interface.


##  Features

- Live chat UI with streaming responses
- Backend powered by **Flask**
- Integration with **Groq's LLaMA 4 model**
- Clean and mobile-responsive design
- Deployable on **Render**, **Railway**, or any Flask-compatible host

---

##  Live Demo

>https://chatbot-3-w1ns.onrender.com/ 

---

##  Project Structure

```


├── app.py               # Flask backend with chat route
├── templates/
│   └── index.html       # Chat UI (auto-rendered by Flask)
├── static/              # (Optional) place CSS/JS here
├── requirements.txt     # Python dependencies
├── Procfile             # For deploying on Render
├── .env                 # Contains your GROQ\_API\_KEY
└── README.md            # Project documentation

````

---

##  Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yusufadepoju1/Chatbot.git
cd ai-assistant-chatbot
````

### 2. Create & Activate a Virtual Environment (Optional but recommended)

```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variable

Create a `.env` file in the root folder:

```bash
echo "GROQ_API_KEY=your-groq-api-key-here" > .env
```

### 5. Run the App Locally

```bash
python app.py
```

Visit `http://localhost:5000` in your browser.

---

## 🌐 Deployment (Render)

### Files required:

* `requirements.txt`
* `Procfile`
* `app.py`
* `templates/index.html`
* `.env` (set GROQ\_API\_KEY in Render environment settings)

### Sample `Procfile`

```
web: gunicorn app:app
```

> Make sure `app.py` contains `app = Flask(__name__)`.

---

##  Example `.env` file

```
GROQ_API_KEY=your_actual_api_key_here
```

---

##  License

This project is licensed under the MIT License — feel free to use, remix, and deploy.

---

## Author

Built by \Yusuf Adepoju
GitHub: [@your-username](https://github.com/yusufadepoju1)


---



