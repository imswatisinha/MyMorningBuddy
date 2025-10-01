# MyMorningBuddy ☀️

**Your Personal Morning Assistant** - Start your day informed and prepared with weather updates, personalized news, and smart day planning powered by AI.

## 📖 Overview

MyMorningBuddy is an intelligent morning companion application that helps you plan and start your day efficiently. It provides real-time weather information with smart suggestions on what to wear, curated news based on your interests, and creates personalized daily itineraries that consider local weather conditions and events happening in your city.

## 🚀 Tech Stack

### Frontend
- **Streamlit** - Interactive web application framework for Python
  - Used for creating the user interface with minimal code
  - Provides responsive design and interactive widgets
  - Handles navigation and page routing

### Backend & APIs
- **Python 3.x** - Core programming language
- **Google Gemini AI (gemini-2.5-flash & gemini-2.5-flash-lite)** - Advanced AI models for:
  - Natural language processing and content generation
  - Weather report interpretation and personalization
  - News summarization
  - Smart itinerary planning with function calling
- **OpenWeather API** - Real-time weather data
- **News API** - Latest news and headlines
- **SerpAPI (Google Events)** - Local event discovery

### Libraries & Dependencies
- **google-genai** - Google's Generative AI SDK for Python
- **requests** - HTTP library for API calls
- **python-dotenv** - Environment variable management
- **datetime** - Date and time operations

## ✨ Key Features

### 1. **Home Page**
- Displays inspirational morning quotes
- Shows beautiful nature images to start your day
- Simple navigation to all features

### 2. **Weather Updates**
- Get current weather for any city worldwide
- Temperature conversion (Kelvin to Celsius)
- Detailed information including:
  - Current and "feels like" temperature
  - Humidity levels
  - Wind speed
  - Sunrise and sunset times
- **AI-Powered Smart Suggestions**:
  - What to wear based on temperature
  - What to carry (umbrella, sunglasses, etc.)
  - Hydration and safety tips

### 3. **News by Interest**
- Personalized news based on your interests (Technology, Sports, Health, etc.)
- Displays top 5 latest articles with:
  - Article title
  - Featured image
  - Article link
  - **AI-Generated Summary** - Quick digest of each article

### 4. **Smart Planner**
- Creates a personalized day itinerary for your city
- Uses AI to combine:
  - Weather forecast for the day
  - Local events and activities
  - Popular tourist attractions
  - Best times for outdoor vs indoor activities
- Provides chronological plan (Morning → Afternoon → Evening)
- Includes:
  - Meal recommendations
  - Event timing and links
  - Weather-appropriate activity suggestions

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip (Python package installer)

### Step 1: Clone the Repository
```bash
git clone https://github.com/imswatisinha/MyMorningBuddy.git
cd MyMorningBuddy
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Set Up Environment Variables
Create a `.env` file in the project root directory and add your API keys:

```env
GOOGLE_API_KEY=your_google_gemini_api_key_here
```

**Note:** The application also uses the following API keys (currently hardcoded in `applications.py`):
- OpenWeather API Key
- News API Key
- SerpAPI Key

### Step 4: Run the Application
```bash
streamlit run app.py
```

The application will open in your default web browser at `http://localhost:8501`

## 📋 Usage Guide

### Getting Weather Information
1. Navigate to "Get Weather of your City" from the sidebar
2. Enter your city name
3. Click "Fetch Information"
4. View detailed weather report with personalized suggestions

### Reading Personalized News
1. Navigate to "News by Interest" from the sidebar
2. Enter your area of interest (e.g., Technology, Sports, Health)
3. Click "Fetch News"
4. Browse through 5 latest articles with AI-generated summaries

### Creating Your Day Plan
1. Navigate to "Smart Planner" from the sidebar
2. Enter your city name
3. Click "Let's Plan"
4. Receive a personalized itinerary considering weather and local events

## 📁 Project Structure

```
MyMorningBuddy/
│
├── app.py                 # Main Streamlit application (UI & routing)
├── applications.py        # Core business logic and API integrations
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
└── .env                  # Environment variables (not in repo)
```

## 🔑 API Keys Required

To run this application, you'll need the following API keys:

1. **Google Gemini API** - Get from [Google AI Studio](https://makersuite.google.com/app/apikey)
2. **OpenWeather API** - Get from [OpenWeatherMap](https://openweathermap.org/api)
3. **News API** - Get from [NewsAPI.org](https://newsapi.org/)
4. **SerpAPI** - Get from [SerpAPI](https://serpapi.com/)

## 🌟 Highlights

- **AI-Powered Intelligence**: Leverages Google Gemini's advanced function calling capabilities
- **Real-Time Data**: Integrates multiple APIs for up-to-date information
- **Personalized Experience**: Tailors recommendations based on user input and context
- **User-Friendly Interface**: Clean and intuitive Streamlit UI
- **Smart Context Awareness**: Weather-appropriate suggestions and planning

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📝 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Swati Sinha**
- GitHub: [@imswatisinha](https://github.com/imswatisinha)

---

**Start your mornings right with MyMorningBuddy! ☀️**
