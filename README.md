# 🟢 Chit Chat - A Real-Time Chat App with Django, WebSocket, and Redis

A simple and practical real-time chat application built using Django, Django Channels, WebSockets, and Redis. This project demonstrates how to implement bi-directional communication between users using asynchronous technologies in Django.

---

## 💡 Features

- 🔄 Real-time messaging with WebSocket
- 🔧 Powered by Django Channels and Redis
- 🎨 Clean UI with Bootstrap 5
- 🧩 Modular and beginner-friendly codebase
- 🐳 Docker support for Redis (optional)

---

## ⚙️ Technologies Used

- **Django** – High-level Python web framework
- **Django Channels** – WebSocket support for Django
- **Channels Redis** – Redis integration for Channels
- **Daphne** – ASGI server to serve async Django
- **Redis** – In-memory data structure store used as a message broker
- **HTML + Bootstrap 5** – Frontend styling
- **Docker (optional)** – To containerize Redis

---

## 🚀 Getting Started

Follow these steps to set up the project locally on your machine:

### 1. Clone the Repository

git clone https://github.com/yourusername/my_secure_journal_app.git
cd my_secure_journal_app

### 2. Create a Virtual Environment and Activate It

python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate

### 3. Install the Requirements

pip install -r requirements.txt

If requirements.txt doesn't exist, install manually:
pip install django channels channels_redis daphne

### 4. Start Redis Server
If you have Redis installed locally:

redis-server

Or run it using Docker:
docker run -p 6379:6379 -d redis

### 5. Run Migrations and Start the Server

python manage.py migrate
python manage.py runserver

### 6. Visit the App
Open your browser and go to:

http://127.0.0.1:8000/
You should now be able to test real-time chat functionality between multiple tabs or devices.

🐳 Optional: Redis via Docker
If you prefer not to install Redis locally:
docker run -p 6379:6379 -d redis

## 📁 Project Structure

ChitChat/  
├── chat/                   # Chat app with routing and consumers  
├── secure_journal_app/     # Main Django project settings  
├── templates/              # HTML templates  
├── static/                 # Static files (CSS, JS)  
├── manage.py               # Django CLI entry  
├── requirements.txt        # Python dependencies  

## 📜 License
This project is open-source and available under the MIT License.

## 🙌 Acknowledgements
Originally inspired by real-time chat apps built with Django and Channels.
