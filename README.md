# WeatherBot

WeatherBot is a simple Flask-based web application that provides weather information and integrates with Dialogflow for chatbot interactions.

## Features

- REST API endpoint for weather queries
- Dialogflow webhook integration
- CORS support for cross-origin requests

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/bhawnadhaka/weatherbot.git
cd weatherbot
```

### 2. Create and Activate a Python Environment

```bash
conda create -p ./weatherbot python=3.7 -y
conda activate ./weatherbot
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

The app will start on [http://localhost:8080](http://localhost:8080).

## API Endpoints

- **GET /**  
  Returns a welcome message.

- **POST /webhook**  
  Accepts JSON requests from Dialogflow and returns weather information.

## Example Dialogflow Request

```json
{
  "queryResult": {
    "parameters": {
      "city_names": "delhi"
    }
  }
}
```

## Git Commands Reference

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/bhawnadhaka/weatherbot.git
git push -u origin main
```

## License

This project is