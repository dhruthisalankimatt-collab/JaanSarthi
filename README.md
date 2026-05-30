# Eco-Grid RESONEX Dashboard

A real-time smart infrastructure monitoring and sustainable energy management dashboard built using **React**, **Vite**, **ESP32-S3**, and **WebSerial API**.

The platform provides live monitoring of structural assets, safety systems, and renewable energy sources through an interactive dashboard.

---

## Features

### Structural Monitoring

- Real-time vibration monitoring
- Flyover health tracking
- Metro pillar monitoring
- Streetlight pole vibration analysis
- Live sensor visualization

### Structural Health Scoring

- AI-based health assessment
- Health score range: 0–100%
- Automatic warning and critical detection

### Smart Guardian System

- PIR motion detection
- Acoustic anomaly detection
- Emergency SOS monitoring
- Real-time safety alerts

### Energy Monitoring

- Solar energy generation tracking
- Wind energy harvesting monitoring
- Battery storage visualization
- Live energy status indicators

### Event & Alert System

- Real-time event logging
- Critical alert notifications
- Historical activity tracking

### Hardware Integration

- ESP32-S3 support
- WebSerial communication
- Plug-and-play device connection
- Live sensor streaming

---

## Tech Stack

| Layer | Technology |
|---------|------------|
| Frontend | React.js |
| Build Tool | Vite |
| Charts | Recharts |
| Icons | Lucide React |
| Communication | WebSerial API |
| Hardware | ESP32-S3 |
| Styling | CSS3 |
| Runtime | Node.js |

---

# Project Setup

## Prerequisites

- Node.js (LTS Version)
- npm
- Google Chrome or Microsoft Edge

Download Node.js:

https://nodejs.org

---

## Create Project

```bash
npm create vite@latest eco-grid-resonex-dashboard -- --template react
cd eco-grid-resonex-dashboard
```

---

## Replace Source Files

Replace the contents of the `src/` directory with:

```text
src/
├── index.css
├── main.jsx
├── App.jsx
├── data/
│   └── mockData.js
├── components/
│   ├── TopBar.jsx
│   ├── MetricCards.jsx
│   ├── VibrationChart.jsx
│   ├── SafetyPanel.jsx
│   ├── EnergyPanel.jsx
│   └── AlertsFeed.jsx
```

Also replace:

```text
package.json
vite.config.js
```

---

## Install Dependencies

```bash
npm install
npm install recharts lucide-react
```

---

## Run Development Server

```bash
npm run dev
```

Open:

```text
http://localhost:5173
```

---

# Hardware Integration

## ESP32-S3 Firmware Upload

Open:

```text
esp32_firmware.ino
```

Upload using Arduino IDE.

### Board Selection

```text
Tools → Board → ESP32S3 Dev Module
```

---

## Connect ESP32

1. Open the dashboard.
2. Click **Connect ESP32**.
3. Select the ESP32 COM port.
4. Allow WebSerial access.

Live sensor data will begin streaming automatically.

---

# Dashboard Modules

## Top Bar

- System status
- Device connection status
- Timestamp information

## Structural Monitoring

- Real-time vibration charts
- Multi-sensor visualization
- Historical trends

## Health Metrics

- Infrastructure health score
- Risk indicators
- Warning thresholds

## Smart Guardian

- Motion detection
- Acoustic monitoring
- SOS event tracking

## Energy Panel

- Solar output
- Wind generation
- Battery level monitoring

## Alerts Feed

- Live notifications
- Critical event logging
- System warnings

---

# System Architecture

```text
ESP32 Sensors
      │
      ▼
WebSerial API
      │
      ▼
React Dashboard
      │
      ▼
Data Processing Layer
      │
      ├── Structural Monitoring
      ├── Health Assessment
      ├── Smart Guardian
      └── Energy Analytics
```

---

# Browser Compatibility

| Browser | Supported |
|----------|----------|
| Chrome | ✅ |
| Edge | ✅ |
| Firefox | ❌ |
| Safari | ❌ |

> WebSerial API currently works only in Chromium-based browsers.

---

# Future Enhancements

- TinyML anomaly detection
- Predictive maintenance analytics
- Smart city integration
- LoRaWAN connectivity
- Mobile application support
- Renewable energy forecasting
- Cloud synchronization

---

# License

Developed as part of the **Eco-Grid RESONEX Initiative**.

© 2026 Eco-Grid RESONEX. All Rights Reserved.
