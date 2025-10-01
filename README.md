
# 🌅 Morning Buddy

A smart daily companion application that helps you start your day right with personalized weather updates, news, and daily planning assistance.

## 🌟 Features

### 1. Smart Dashboard
- Beautiful morning quotes and inspiring images
- Clean, intuitive interface with easy navigation
- Responsive design for all device sizes

### 2. Weather Intelligence 🌤️
- Real-time weather updates for any city
- Temperature in Celsius with detailed metrics
- Smart clothing and accessory recommendations based on weather conditions
- Powered by OpenWeather API

### 3. Personalized News Feed 📰
- Interest-based news curation
- Top 5 latest articles with images
- AI-powered news summarization
- News from various categories (Technology, Sports, Health, etc.)
- Powered by NewsAPI

### 4. Smart Day Planner 📅
- AI-powered day planning based on:
  - Local weather forecast
  - City events and activities
  - Tourist attractions
  - Local dining recommendations
- Interactive scheduling
- Real-time event updates
- Powered by Google Events API

## 🛠️ Tech Stack

### Frontend
- Streamlit - For the interactive web interface
- HTML/CSS - For custom styling and layouts

### Backend
- Python 3.x
- Key Libraries:
  - `streamlit` - Web application framework
  - `requests` - HTTP requests handling
  - `python-dotenv` - Environment variable management
  - `google.genai` - Google's Generative AI integration

### APIs
- OpenWeather API - Weather data
- NewsAPI - Current news fetching
- Google Generative AI (Gemini) - Content generation and summarization
- SerpAPI - Local events data

### AI/ML
- Google Gemini 2.5 Flash - For:
  - News summarization
  - Weather interpretation
  - Smart planning suggestions
  - Content generation

## 🚀 Getting Started

1. Clone the repository
```bash
git clone https://github.com/yourusername/morning-buddy.git
cd morning-buddy
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Set up environment variables
Create a `.env` file in the root directory and add your API keys:
```env
GOOGLE_API_KEY=your_google_api_key
```

4. Run the application
```bash
streamlit run app.py
```

## 📱 Usage

1. **Home Page**
   - View inspirational quotes
   - See beautiful morning images
   - Access quick navigation to all features

2. **Weather Updates**
   - Enter your city name
   - Get detailed weather information
   - Receive personalized recommendations

3. **News Section**
   - Enter your interests
   - View latest news with summaries
   - Click through to full articles

4. **Smart Planner**
   - Enter your city
   - Get AI-generated day plans
   - View local events and activities

## 🔑 API Keys Required
- Google API Key (for Gemini AI)
- OpenWeather API Key
- NewsAPI Key
- SerpAPI Key

## 🤝 Contributing
Contributions, issues, and feature requests are welcome!

## Link
https://mymorningbuddy-g9atx39xpzxpiptshtogb4.streamlit.app/

## 📝 License
This project is [MIT](https://choosealicense.com/licenses/mit/) licensed.
