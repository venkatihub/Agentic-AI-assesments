Here's a complete **`README.md`** file for your **Intelligent Travel Assistant** app powered by Gemini, LangChain, and DuckDuckGo:

---

# 🌍 Intelligent Travel Assistant AI

Your smart AI travel planner powered by **Gemini**, **LangChain**, and **Streamlit**!
Get personalized travel information including **weather**, **attractions**, **hotel recommendations**, and **tips**—all tailored to your **destination**, **style**, and **budget** in a beautifully conversational chat format.

---

## ✨ Features

* 🧠 **LLM-powered Chat**: Uses Google's Gemini 2.5 Flash model for intelligent responses.
* ☀️ **Live Weather Data**: Gets real-time weather from **WeatherAPI** and **OpenWeatherMap** (as fallback).
* 🏞️ **Top Attractions**: Scrapes and summarizes must-see places using DuckDuckGo and Gemini.
* 🏨 **Stay Recommendations**: Suggests accommodations tailored to your **travel style** and **budget**.
* 💬 **Conversational Interface**: Enjoy natural chat-like interaction with an AI assistant.
* 🔧 **Built-in Tools**: All tasks are modular and reusable using LangChain’s `@tool` decorators.

---

## 🖥️ Interface Overview

| Component       | Description                                  |
| --------------- | -------------------------------------------- |
| **Sidebar**     | Set destination, style, duration, and budget |
| **Chat Window** | Interact with the assistant in real-time     |
| **Debug Panel** | View intermediate reasoning and tool outputs |
| **Footer**      | Attribution and branding                     |

---

## 🧠 Powered By

* [🌟 Gemini (Google Generative AI)](https://deepmind.google/technologies/gemini)
* [🔗 LangChain](https://www.langchain.com/)
* [🦆 DuckDuckGo Search API](https://duckduckgo.com/)
* [🌦️ WeatherAPI](https://www.weatherapi.com/) & [🌩️ OpenWeatherMap](https://openweathermap.org/)
* [📦 Streamlit](https://streamlit.io/)

---

## ⚙️ Setup & Installation

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/intelligent-travel-assistant.git
cd intelligent-travel-assistant
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Add API Keys

You can hardcode them or set them via `.env`:

```
GEMINI_API_KEY=your_gemini_key
WEATHER_API_KEY=your_weatherapi_key
```

Or replace them directly in the script.

### 4. Run the App

```bash
streamlit run your_script_name.py
```

---

## 🧰 Tools Used

```python
@tool
def get_current_weather(location: str) -> str
```

Fetches weather using WeatherAPI and falls back to OpenWeatherMap.

```python
@tool
def get_top_attractions(location: str) -> str
```

Uses DuckDuckGo + Gemini to list 5 top attractions.

```python
@tool
def get_accommodation_recommendations(location: str, travel_style: str) -> str
```

Finds best accommodations tailored to your travel style and location.

---

## 📦 Key Libraries

```text
streamlit
langchain
langchain-google-genai
langchain-community
duckduckgo-search
requests
```

Install with:

```bash
pip install streamlit langchain langchain-google-genai langchain-community duckduckgo-search requests
```

---

## 💬 Sample Chat

> **You:** I’m planning a cultural 5-day trip to Chennai with a mid-range budget.
>
> 🤖 **Assistant:**
>
> ### Weather Report ☀️
>
> Sunny and humid, \~33°C. Feels like 36°C.
>
> ### Top Attractions 🏰
>
> 1. **Kapaleeshwarar Temple** (Temple) - Historic Dravidian architecture. Why visit: Spiritual and architectural value.
> 2. **Marina Beach** (Beach) - India’s longest beach. Why visit: Scenic sunrise and snacks.
>    ...
>
> ### Where to Stay 🛏️
>
> 1. **Hotel RainTree** (Hotel) - Rooftop pool, central location. Why good: Affordable luxury for cultural explorers.
>    ...
>
> ### Travel Tips 💡
>
> * Carry cotton clothes
> * Use Ola/Uber instead of public buses
> * Visit temples early morning

---

## 📸 UI Snapshot

*You can add a screenshot here if desired for visual reference.*

---

## 🙋‍♂️ Authors

**Created by**: Venkateshwaran A
**Team**: SNSIHUB
*Assisted by Gemini + LangChain*

---

## 📃 License

This project is licensed under MIT. Free to use and customize.

---

Would you like me to generate a fancy badge section or auto-generate a `requirements.txt` from the code as well?
