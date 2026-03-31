# ✈️ AI Travel Planner

A Flask-based web application that generates personalized travel itineraries using the OpenTripMap API. Enter a city, number of days, and your interests — and get a curated day-by-day plan along with nearby hotels, shopping spots, hospitals, and wellness centers.

---

## 🌟 Features

- **Smart Itinerary Generator** — Day-by-day travel plan based on your interests
- **Hotel Recommendations** — Find nearby accommodations
- **Shopping Spots** — Discover local markets and malls
- **Nearby Hospitals** — Stay safe with emergency info
- **Wellness & Treatment** — Spas, yoga retreats, and health centers
- **Interest-based Filtering** — Adventure, Religious, or Nature trips
- **Beautiful Dark UI** — Luxury travel aesthetic with responsive design

---

## 🗂️ Project Structure

```
travel-planner/
├── app.py               ← Flask backend & API logic
├── templates/
│   └── index.html       ← Frontend (HTML + CSS combined)
└── README.md
```

---

## ⚙️ Requirements

- Python 3.7+
- Flask
- Requests

---

## 📦 Installation

**1. Clone or download the project**

```bash
git clone https://github.com/yourusername/ai-travel-planner.git
cd ai-travel-planner
```

**2. Install dependencies**

```bash
pip install flask requests
```

**3. Add your API key**

Open `app.py` and replace the API key on this line:

```python
OPENTRIP_API_KEY = "your_api_key_here"
```

Get a free key at: https://opentripmap.io/product

---

## 🚀 Running the App

```bash
python app.py
```

Then open your browser and go to:

```
http://127.0.0.1:5000
```

---

## 🧠 How It Works

1. User enters a **city name**, **number of days**, and **interest** (Adventure / Religious / Nature)
2. The app calls the **OpenTripMap Geoname API** to get the city's coordinates
3. It then fetches nearby **attractions, hotels, shops, hospitals, and wellness centers**
4. A simple **rule-based AI** filters attractions by matching keywords to the selected interest
5. A **day-by-day itinerary** is generated and displayed along with all other categories

---

## 🔑 API Used

| API | Purpose | Link |
|-----|---------|------|
| OpenTripMap | Places, attractions, hotels, hospitals | https://opentripmap.io |

---

## 🎨 Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Flask |
| Frontend | HTML, CSS (Cormorant Garamond + Outfit fonts) |
| API | OpenTripMap REST API |
| Templating | Jinja2 (Flask) |

---

## 📸 UI Preview

The app features a dark luxury travel aesthetic with:
- Gold accent colors on a deep navy background
- Two-column results grid for hotels, shopping, hospitals & wellness
- Color-coded sections for easy scanning
- Fully responsive layout

---

## ⚠️ Known Limitations

- OpenTripMap free tier has rate limits (1 request/second)
- Some smaller cities may return limited results
- Hotel/shop data depends on OpenTripMap's coverage for that region
- The AI recommendation is rule-based (keyword matching), not ML-powered

---

## 🛠️ Future Improvements

- Integrate Google Places API for richer hotel/shop data
- Add weather forecast for travel dates
- Export itinerary as PDF
- Add map view using Leaflet.js
- User login to save past trips

---

## 📄 License

This project is open source and free to use for personal and educational purposes.

---

## 🙋 Author

Built with Flask + OpenTripMap API.  
Feel free to contribute or raise issues!
