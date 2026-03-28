# OCEANUS — Live Maritime Intelligence

A real-time AIS vessel tracking dashboard powered by [AISStream.io](https://aisstream.io).

🌐 **Live at:** `https://YOUR-USERNAME.github.io/oceanus`

---

## Features

- 🛳️ Real-time vessel positions via AISStream.io WebSocket
- 🔍 Search by vessel name, MMSI, IMO, or callsign
- 🎛️ Filter by vessel type (Cargo, Tanker, Passenger, Fishing, Tug, Military)
- 📍 Click any vessel for full details + position history trail
- 🗺️ Dark Leaflet map with 12 major port quick-nav buttons
- 🔄 Auto-resubscribes to current map viewport as you pan/zoom
- 💾 API key saved in localStorage — reconnects automatically

---

## Setup

### 1. Get a free AISStream API key
- Go to [aisstream.io](https://aisstream.io)
- Create a free account
- Dashboard → API Keys → Generate Key

### 2. Deploy to GitHub Pages
- Push this repo to GitHub
- Go to **Settings → Pages → Source → Deploy from branch → main → / (root)**
- Wait ~60 seconds for it to go live

### 3. Open your site
- Visit `https://YOUR-USERNAME.github.io/oceanus`
- Paste your API key when prompted
- The key is saved in your browser — won't ask again

---

## Running locally (optional)

Because WebSockets require HTTPS or localhost, you need a local server:

```bash
# Python
python3 -m http.server 8080
# then open http://localhost:8080
```

---

## Data Source

Vessel positions from the global AIS (Automatic Identification System) network via [AISStream.io](https://aisstream.io).  
Map tiles by [CartoDB](https://carto.com).
