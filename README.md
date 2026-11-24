<div align="center">

<img src="./icon.png" width="120" height="120" alt="Indian Railways API Logo" style="border-radius: 50%; box-shadow: 0 4px 12px rgba(0,0,0,0.15);" />

# Indian Railways Real-Time API
### Official Live Train Status, Timetables & Station Boards for Developers

[![Apify Actor](https://img.shields.io/badge/Apify-Actor%20Live-brightgreen?style=for-the-badge&logo=apify)](https://console.apify.com/actors/KsTj77ESQzY256FEj)
[![Standby Mode](https://img.shields.io/badge/Standby-Sub--Second%20Latency-blue?style=for-the-badge)](https://krawlo--indian-railways-realtime-api.apify.actor)
[![Zero CAPTCHA](https://img.shields.io/badge/Zero-CAPTCHAs-orange?style=for-the-badge)](https://console.apify.com/actors/KsTj77ESQzY256FEj)
[![Protocol](https://img.shields.io/badge/Protocol-REST%20%7C%20MCP%20%7C%20Standby-purple?style=for-the-badge)](https://console.apify.com/actors/KsTj77ESQzY256FEj)

[**🚀 Try Live on Apify Console**](https://console.apify.com/actors/KsTj77ESQzY256FEj) • [**⚡ Live Standby Server Endpoint**](https://krawlo--indian-railways-realtime-api.apify.actor) • [**💻 GitHub Repository**](https://github.com/krawlo/indian-railways-scraper)

**The most affordable, high-speed, and reliable Indian Railways train data API on the market.**  
Integrate official live train tracking, schedule timetables, station-to-station searches, and live departure boards into your travel apps, dashboards, chatbots, and automation workflows.

</div>

---

## 🔗 Quick Links

| Platform / Interface | URL / Endpoint |
| :--- | :--- |
| **Apify Actor Console** | [https://console.apify.com/actors/KsTj77ESQzY256FEj](https://console.apify.com/actors/KsTj77ESQzY256FEj) |
| **Live Standby Server** | [https://krawlo--indian-railways-realtime-api.apify.actor](https://krawlo--indian-railways-realtime-api.apify.actor) |
| **GitHub Repository** | [https://github.com/krawlo/indian-railways-scraper](https://github.com/krawlo/indian-railways-scraper) |

---

## ⚡ Why Use This Actor?

- 🚀 **Sub-Second Standby Mode:** Supports Apify Standby mode for instant, real-time HTTP queries without cold starts.
- 🕒 **Official Real-Time Accuracy:** Direct source updates for train delays, platform numbers, and coach positions.
- 💰 **Unbeatable Pricing:** Transparent, pay-as-you-go pricing designed for developers and scale.
- 🤖 **AI & Agent Ready:** Includes a native **Model Context Protocol (MCP)** server interface for Claude, Cursor, and ChatGPT.
- 🔒 **Zero Blockages:** Pre-configured with automatic retry backoff, circuit breaking, and country-level proxy routing.

---

## 💎 Transparent, Developer-Friendly Pricing

Pay only for what you query. No expensive monthly minimums, no lock-in, and full platform usage transparency:

| Plan / Tier | Price | Included Queries | Cost Per Query | Best For |
| :--- | :--- | :--- | :--- | :--- |
| **Starter** | **$0.85 + usage** | **1,000 Requests** | **$0.00085** | Prototypes, side projects & daily alerts |
| **Growth** | **$3.20 + usage** | **4,000 Requests** | **$0.00080** | Travel portals, mobile apps & automation |
| **Scale** | **$7.50 + usage** | **10,000 Requests** | **$0.00075** | High-volume production & booking engines |

> 💡 **Why this is unbeatable:** Commercial railway APIs on RapidAPI charge **$15.00 to $25.00/month** for only 1,000 requests ($0.015 - $0.025 per request). Our Actor gives you **95% savings** with direct real-time accuracy, official coach compositions, and zero CAPTCHAs.

---

## 🎯 What You Can Query

### 1. 🕒 Live Train Running Status (`LIVE_STATUS`)
Track any Indian Railways train in real time:
- Current running status and delay in minutes (late / on-time).
- Last departed station and upcoming station with estimated arrival (ETA) and departure (ETD).
- Assigned platform numbers at each stoppage.
- Complete train rake and coach composition (e.g. `B1-B2-B3...H1-A1-A2...`).

### 2. 🗺️ Official Train Timetable & Route (`TRAIN_SCHEDULE`)
Fetch the complete master route for any 5-digit train number:
- All stoppage stations with scheduled arrival and departure times.
- Distance from origin in kilometers and halt durations.
- Operating days (Daily, Mon-Sun) and available classes (`1A`, `2A`, `3A`, `SL`, etc.).
- Bilingual station and train names (English & Hindi).

### 3. 🚉 Station-to-Station Train Search (`TRAINS_BETWEEN_STATIONS`)
Find all direct trains operating between two railway stations:
- Origin and destination station codes (e.g. `NDLS` to `MMCT`).
- Departure time, arrival time, and total travel duration.
- Weekly running calendar and train types (Rajdhani, Shatabdi, Superfast, Mail/Express).

### 4. 📋 Live Station Departure & Arrival Board (`STATION_LIVE_BOARD`)
Instant station board for any railway terminal in India:
- See all trains arriving and departing in the upcoming **2, 4, or 8 hours**.
- Live delay status (`On Time`, `Late by 15 min`) and platform assignments.
- Cancellation and diversion alerts.

### 5. 💺 Coach Position Finder (`COACH_POSITION`)
Fetch complete coach composition and platform position:
- Coach sequence (e.g. `ENG`, `LPR`, `BE1`, `B1`, `B2`, `PC`, `H1`, `A1`, `VP`).
- Engine position (`Front` or `Rear`).
- Approximate coach location on platform (`Front (Engine End)`, `Middle`, `Rear (Guard End)`).
- Breakdown of coach classes and types (Engine, Sleeper, 3A, 2A, 1A, Pantry, Parcel).

### 6. ⏱️ Intermediate Station ETA & Stoppage Delay (`INTERMEDIATE_STATION_ETA`)
Predict when a train will reach an intermediate stoppage station along its route:
- Target station scheduled vs estimated arrival (STA / ETA) and departure (STD / ETD).
- Real-time delay in minutes and arrival/departure status (`Expected`, `Arrived / At Platform`, `Departed`).
- Platform number and distance in kilometers.

### 7. 🚨 Platform Change Alerts (`PLATFORM_ALERTS`)
Detect station platform changes automatically:
- Checks announced platform against user's expected platform.
- Flags platform anomalies (`is_platform_changed: true`) with alert notices.

---

## 🛠️ How to Use

### Option 1: Run via Apify Console UI
1. Open the [Actor in Apify Console](https://console.apify.com/actors/KsTj77ESQzY256FEj).
2. Select your **Operation Mode** from the dropdown (`LIVE_STATUS`, `TRAIN_SCHEDULE`, etc.).
3. Enter your **5-digit Train Number** (e.g. `12951`) or **Station Codes** (e.g. `NDLS`, `MMCT`).
4. Click **Start** to run and view the results in the Dataset tab or download as JSON/CSV/Excel.

---

### Option 2: Call via Python (`apify-client`)

```python
from apify_client import ApifyClient

client = ApifyClient("YOUR_APIFY_API_TOKEN")

# Example: Get Live Running Status of Mumbai Rajdhani (12951)
run_input = {
    "action": "LIVE_STATUS",
    "trainNumbers": ["12951"]
}

# Run the Actor and fetch results
run = client.actor("krawlo/indian-railways-realtime-api").call(run_input=run_input)
for item in client.dataset(run["defaultDatasetId"]).iterate_items():
    print(f"Train: {item['train_name']} | Current Delay: {item['current_delay']} min")
    print(f"Last Visited Station: {item['last_station_name']}")
```

---

### Option 3: Call via Node.js / JavaScript

```javascript
import { ApifyClient } from 'apify-client';

const client = new ApifyClient({
    token: 'YOUR_APIFY_API_TOKEN',
});

// Example: Search Trains Between New Delhi (NDLS) and Mumbai Central (MMCT)
const input = {
    action: "TRAINS_BETWEEN_STATIONS",
    fromStation: "NDLS",
    toStation: "MMCT"
};

const run = await client.actor("krawlo/indian-railways-realtime-api").call(input);
const { items } = await client.dataset(run.defaultDatasetId).listItems();
console.log(`Found ${items.length} trains running today:`);
console.table(items.slice(0, 5));
```

---

### Option 4: Instant cURL / REST API

```bash
curl --request POST \
  --url "https://api.apify.com/v2/acts/krawlo~indian-railways-realtime-api/run-sync-get-dataset-items?token=YOUR_API_TOKEN" \
  --header "Content-Type: application/json" \
  --data '{
    "action": "LIVE_STATUS",
    "trainNumbers": ["12951"]
  }'
```

---

## 📊 Sample Output (Live Running Status)

```json
{
  "query_type": "LIVE_STATUS",
  "train_number": "12951",
  "train_name": "NDLS TEJAS RAJ",
  "train_hindi_name": "तेजस राजधानी",
  "source_station_name": "MUMBAI CENTRAL",
  "destination_station_name": "NEW DELHI",
  "journey_start_date": "20-Nov-2026",
  "last_station_name": "VADODARA JN",
  "current_delay": "0",
  "total_distance_km": 1380,
  "total_stoppages": 8,
  "stoppages": [
    {
      "station_code": "BRC",
      "station_name": "VADODARA JN",
      "platform": "2",
      "scheduled_arrival": "21:06",
      "scheduled_departure": "21:16",
      "delay_arrival": "On Time",
      "coach_position": "ENG-LPR-BE1-B1-B2-B3-B4-B5-B6-B7-B8-B9-B10-B11-PC-H1-A1-A2-A3-A4-A5-LPR-VP"
    }
  ]
}
```

---

## ⚡ Standby Mode (Real-Time Web API with Smart Auto-Sleep)

This Actor supports **Apify Standby Mode**. When enabled:
- The container remains warm in the background ready to answer queries in **< 1 second**.
- **Smart Idle Timeout (`idleTimeoutSecs: 90`):** Automatically shuts down after 90 seconds of inactivity (configurable between 60s and 120s), guaranteeing you never pay for unused idle compute credits!
- You can send HTTP requests directly to the Actor's web server URL with **sub-second latency**:
  ```bash
  curl -X POST "https://krawlo--indian-railways-realtime-api.apify.actor/" \
    -H "Content-Type: application/json" \
    -d '{"action": "LIVE_STATUS", "trainNumber": "12951"}'
  ```
- Perfect for real-time mobile travel apps, WhatsApp bots, and Telegram notification bots.

---

## 🤖 Connect to AI Assistants (MCP Server)

You can run this project as a native **Model Context Protocol (MCP)** server for AI coding assistants and chatbots:
```bash
python -m src.mcp_server
```

### Claude Desktop / Cursor / Antigravity Configuration
Add the server configuration to your `claude_desktop_config.json`, `mcp.json`, or Antigravity MCP settings:

```json
{
  "mcpServers": {
    "indian-railways": {
      "command": "python",
      "args": ["-m", "src.mcp_server"],
      "cwd": "/path/to/indian-railways-scraper",
      "env": {
        "PYTHONUNBUFFERED": "1",
        "HTTPS_PROXY": "http://user:pass@proxy.example.com:8000"
      }
    }
  }
}
```

> 💡 **Tip:** If running outside India, configure `HTTPS_PROXY` (or `RAILWAY_PROXY_URL`) pointing to an Indian proxy to ensure official CRIS/NTES server accessibility.

### Available MCP Tools

| Tool Name | Parameters | Description |
| :--- | :--- | :--- |
| `get_live_running_status` | `train_number`, `date` (optional) | Live running status, delay, last/next station, and stoppage timetable. |
| `get_train_schedule` | `train_number` | Master timetable route, stoppage timings, halt duration, and distance. |
| `get_trains_between_stations` | `from_station`, `to_station`, `train_type` | Find all direct trains between two station codes. |
| `get_live_station_board` | `station_code`, `hours` (2, 4, 8) | Live arrivals and departures board for a station. |
| `get_coach_position` | `train_number`, `station_code` (optional) | Coach composition sequence, engine location, and approximate platform positions. |
| `get_intermediate_station_eta` | `train_number`, `station_code`, `date` | Scheduled vs estimated arrival/departure and delays for a specific stoppage. |
| `get_platform_alerts` | `station_code`, `train_number`, `expected_platform` | Detect platform announcements and check for platform changes. |

Compatible out-of-the-box with **Claude Desktop, Cursor, Antigravity, and LibreChat**.

---

## 🤝 Support & Feature Requests

Need a dedicated quota, custom railway data integrations, or assistance setting up automation?  
Reach out via the **Apify Actor discussion tab** or open an issue on the repository: [https://github.com/krawlo/indian-railways-scraper](https://github.com/krawlo/indian-railways-scraper).
