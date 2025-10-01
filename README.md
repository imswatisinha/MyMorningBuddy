# MyMorningBuddy ☀️

Your intelligent morning companion that provides personalized weather updates, curated news, and smart daily plans to kickstart your day with confidence!

## 🌟 Overview

MyMorningBuddy is an AI-powered web application built with Streamlit that helps you start your day right by providing:
- Real-time weather updates with personalized clothing suggestions
- Curated news based on your interests with AI-powered summaries
- Smart daily planner that combines weather, local events, and tourist attractions
- Inspirational morning quotes and beautiful imagery

## 🚀 Tech Stack

### Frontend
- **[Streamlit](https://streamlit.io/)** - Interactive web application framework for Python
  - Provides the entire UI/UX layer
  - Handles user input and displays dynamic content
  - Multi-page navigation with sidebar

### Backend & APIs
- **[Google Generative AI (Gemini)](https://ai.google.dev/)** - Advanced AI model integration
  - `gemini-2.5-flash` model for natural language processing
  - `gemini-2.5-flash-lite` for optimized responses
  - Function calling capabilities for tool integration
  - Used for:
    - Weather data interpretation and formatting
    - News summarization
    - Smart itinerary planning
    - Natural language responses

- **[OpenWeather API](https://openweathermap.org/api)** - Real-time weather data
  - Current weather conditions
  - Temperature, humidity, wind speed
  - Sunrise and sunset times

- **[News API](https://newsapi.org/)** - Latest news headlines
  - Fetches top 5 latest articles by topic
  - Provides article titles, images, and URLs
  - Sorted by publication date

- **[SerpAPI](https://serpapi.com/)** - Local events search
  - Google Events engine integration
  - Finds upcoming events in specified cities
  - Provides event details, timing, and links

### Core Libraries
- **[Python-dotenv](https://pypi.org/project/python-dotenv/)** - Environment variable management
  - Secure API key storage
  - Configuration management

- **[Requests](https://requests.readthedocs.io/)** - HTTP library
  - API calls to external services
  - Error handling for network requests

- **Python Standard Library**
  - `os` - Environment variable access
  - `random` - Random quote and image selection
  - `datetime` - Date handling for forecasts

## ✨ Features

### 1. Home Page
- **Inspirational Quotes**: Start your day with motivational morning quotes
- **Beautiful Imagery**: Random nature and sunrise images from Unsplash
- **Simple Navigation**: Easy-to-use sidebar for accessing all features

### 2. Weather Updates
- **Current Weather**: Get real-time weather for any city worldwide
- **Smart Suggestions**: AI-powered recommendations on what to wear and carry based on:
  - Temperature (hot, cold, moderate)
  - Weather conditions (rain, clouds, clear)
  - Humidity levels
  - Wind conditions
- **Human-Friendly Format**: Natural language weather reports with Celsius temperatures
- **Complete Information**: 
  - Current and feels-like temperature
  - Weather description
  - Humidity and wind speed
  - Sunrise and sunset times

### 3. News by Interest
- **Personalized News**: Enter any topic (Technology, Sports, Health, etc.)
- **Latest Headlines**: Get the 5 most recent articles
- **Visual Display**: News cards with images and titles
- **AI Summaries**: Gemini-powered concise summaries of each article
- **Direct Links**: Quick access to full articles
- **Multi-Column Layout**: Easy browsing of multiple stories at once

### 4. Smart Planner
- **Intelligent Itinerary**: AI-generated daily plans tailored to your city
- **Weather-Aware Planning**: Suggests indoor/outdoor activities based on forecast
- **Local Events Integration**: Includes nearby events with timing and links
- **Tourist Attractions**: Recommends popular places to visit
- **Balanced Schedule**: Combines sightseeing, events, and meal breaks
- **Chronological Organization**: Morning, afternoon, and evening activities
- **Flexible Options**: Presents multiple choices when available

## 📋 Prerequisites

- Python 3.7 or higher
- API Keys (required):
  - Google Generative AI API key (Gemini)
  - OpenWeather API key
  - News API key
  - SerpAPI key

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/imswatisinha/MyMorningBuddy.git
   cd MyMorningBuddy
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   
   Create a `.env` file in the root directory:
   ```env
   GOOGLE_API_KEY=your_google_gemini_api_key
   ```

   **Note**: Other API keys are currently hardcoded in `applications.py`. For production use, move them to the `.env` file:
   ```env
   OPENWEATHER_API_KEY=your_openweather_api_key
   NEWS_API_KEY=your_news_api_key
   SERPAPI_KEY=your_serpapi_key
   ```

## 🎯 Usage

1. **Start the application**
   ```bash
   streamlit run app.py
   ```

2. **Access the application**
   - Open your browser and navigate to `http://localhost:8501`
   - The app will automatically open in your default browser

3. **Navigate through features**
   - Use the sidebar to switch between pages
   - Enter city names or topics as prompted
   - Click buttons to fetch information

## 📁 Project Structure

```
MyMorningBuddy/
├── app.py                 # Streamlit frontend application
├── applications.py        # Backend functions and API integrations
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables (create this)
└── README.md             # Project documentation
```

## 🔧 Configuration

### API Keys Setup

1. **Google Gemini API**
   - Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create a new API key
   - Add to `.env` file

2. **OpenWeather API**
   - Sign up at [OpenWeather](https://openweathermap.org/api)
   - Get your free API key
   - Update in `applications.py` or `.env`

3. **News API**
   - Register at [News API](https://newsapi.org/)
   - Get your API key
   - Update in `applications.py` or `.env`

4. **SerpAPI**
   - Sign up at [SerpAPI](https://serpapi.com/)
   - Get your API key
   - Update in `applications.py` or `.env`

## 🎨 Features in Detail

### AI-Powered Intelligence
The application leverages Google's Gemini AI model for:
- **Natural Language Processing**: Converting raw API data into human-friendly text
- **Context-Aware Suggestions**: Providing practical advice based on weather conditions
- **Content Summarization**: Condensing news articles into key points
- **Smart Planning**: Creating personalized itineraries considering multiple factors

### Function Calling
The app uses Gemini's function calling feature to:
- Invoke external APIs (weather, events) on demand
- Process real-time data within AI responses
- Generate dynamic, contextual plans

### Error Handling
- Graceful error messages for missing inputs
- Try-except blocks for API failures
- User-friendly error notifications in the UI

## 🌐 Key Integrations

| Integration | Purpose | Usage |
|-------------|---------|-------|
| Google Gemini | AI processing & generation | Weather interpretation, news summaries, smart planning |
| OpenWeather | Weather data | Current conditions, forecasts |
| News API | News content | Latest headlines by topic |
| SerpAPI | Local events | Event discovery and details |
| Unsplash | Images | Morning inspiration photos |

## 🔐 Security Notes

- Store all API keys in `.env` file
- Never commit `.env` to version control
- Add `.env` to `.gitignore`
- Consider using environment variables in production
- Implement rate limiting for API calls

## 🚧 Future Enhancements

- User authentication and personalization
- Saved preferences and favorite cities
- Calendar integration for events
- Multi-day weather forecasts
- Email/notification support for daily briefings
- Mobile-responsive design improvements
- Offline mode for basic features

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

**Swati Sinha**
- GitHub: [@imswatisinha](https://github.com/imswatisinha)

## 🙏 Acknowledgments

- Streamlit for the amazing web framework
- Google for the powerful Gemini AI model
- OpenWeather, News API, and SerpAPI for their excellent APIs
- Unsplash for beautiful free images

---

**Made with ❤️ to make your mornings better!**
