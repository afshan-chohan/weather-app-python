# 🌦️ Weather Web App — Python + Flask + OpenWeather API

A real-time weather web application built with Python and Flask. Users can search any city in the world and instantly view live weather data fetched from the OpenWeather API.

---

## 📌 Project Overview

This project demonstrates backend web development with Python Flask, real-world API integration, JSON data handling, and frontend rendering with HTML/CSS templates — skills directly relevant to building data-driven web applications.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🌍 City Search | Look up real-time weather for any city worldwide |
| 🌡️ Temperature | Displays current temperature in Celsius |
| ☁️ Weather Condition | Shows condition — clear, cloudy, rain, etc. |
| 💧 Humidity | Displays current humidity percentage |
| ⚠️ Error Handling | Graceful messages for invalid or unknown cities |
| 🎨 Clean UI | Simple, user-friendly web interface |
| ☁️ Deployment Ready | Includes Procfile for cloud platform deployment |

---

## 🛠️ Tech Stack

- **Backend:** Python 3, Flask
- **API:** OpenWeatherMap API (live data)
- **Data Format:** JSON (API response parsing)
- **Frontend:** HTML5, CSS3 (Jinja2 templates)
- **Deployment:** Procfile (PythonAnywhere / Heroku compatible)
- **Libraries:** Requests

---

## 📂 Project Structure

```
weather-app-python/
│
├── templates/
│   └── index.html         # Frontend UI — Jinja2 template
├── app.py                 # Flask app — routes, API calls, JSON parsing
├── requirements.txt       # Python dependencies
├── procfile               # Deployment configuration
└── README.md
```

---

## 🧠 How It Works

```
User enters city name
       ↓
Flask receives POST request
       ↓
Python sends GET request to OpenWeather API
       ↓
API returns JSON response with weather data
       ↓
Flask extracts temperature, condition, humidity
       ↓
Jinja2 renders results on the web page
```

---

## ▶️ How to Run Locally

**1. Clone the repository**
```bash
git clone https://github.com/afshan-chohan/weather-app-python.git
cd weather-app-python
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Get a free API key**
- Sign up at [openweathermap.org](https://openweathermap.org/api)
- Copy your API key from the dashboard

**4. Add your API key**

Open `app.py` and replace the API key placeholder:
```python
API_KEY = "0971f17a69c892069ca6d5e5ae40992e"
```

**5. Run the app**
```bash
python app.py
```

**6. Open in browser**
```
http://127.0.0.1:5000
```

---

## 🌐 API Integration

This app uses the **OpenWeatherMap Current Weather API**:

```
GET https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}&units=metric
```

**Sample JSON response parsed by the app:**
```json
{
  "name": "Karachi",
  "main": {
    "temp": 34.2,
    "humidity": 65
  },
  "weather": [
    { "description": "clear sky" }
  ]
}
```

---

## ☁️ Deployment

This project includes a `Procfile` for deployment on cloud platforms:

```
web: python app.py
```

Compatible with **PythonAnywhere**, **Heroku**, and similar platforms.

---

## 📦 Requirements

```
flask
requests
```

---

## 💡 What I Learned

- Building a backend web application with Python Flask
- Consuming a third-party REST API and handling JSON responses
- Passing data from Python to HTML using Jinja2 templating
- Implementing error handling for invalid user inputs
- Structuring a deployable Python web application with a Procfile

---

## 🔮 Future Improvements

- [ ] Add 5-day weather forecast view
- [ ] Display weather icons from the API
- [ ] Add temperature unit toggle (Celsius / Fahrenheit)
- [ ] Store search history using SQLite
- [ ] Deploy live on PythonAnywhere with a public URL

---

## 👩‍💻 Author

**Afshan Chohan**
MSc Data Engineering & Information Management | AWS Cloud Practitioner

🔗 [LinkedIn](https://www.linkedin.com/in/afshan-chohan/) · [GitHub](https://github.com/afshan-chohan)
