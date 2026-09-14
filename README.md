
# 🚦 Tracko — AI-Powered Urban Mobility Intelligence Platform

> **Turning public buses into mobile sensing units for smarter, safer and more responsive cities.**

Tracko is an AI-powered urban intelligence platform designed for Smart India Hackathon 2026.

It combines **public transport intelligence, real-time mobility data and computer vision** to transform city buses into mobile sensing units.

As buses travel through the city, their onboard cameras can continuously observe road conditions. AI models such as YOLO can identify road-level events such as potholes, construction zones, obstructions and other urban anomalies.

These observations are converted into structured geospatial events and delivered to a centralized Tracko platform for monitoring, verification and response.

---

## 🎯 Problem

Urban authorities often receive fragmented, delayed or manually reported information about road conditions and mobility problems.

At the same time, public buses continuously travel across large portions of the city.

Tracko addresses this opportunity by using buses as **mobile urban sensors**.

Instead of deploying dedicated sensing infrastructure everywhere:

**Existing Mobility Infrastructure + AI Vision = Continuous Urban Intelligence**

---

## 💡 Solution

Tracko consists of two major layers:

### 1. Centralized Urban Intelligence Platform

The Tracko platform provides:

* 🚌 Public transport monitoring
* 🗺️ Geospatial incident visualization
* 🚧 Road-condition intelligence
* 📊 Urban mobility analytics
* 🔔 Incident alerts
* 📍 Location-based event tracking
* 📈 Historical event analysis

### 2. AI Mobility Sensing Layer

Bus dashcams provide visual information that can be processed by a YOLO-based computer vision pipeline.

## 🤖 AI Detection

The AI layer is designed to support detection of urban road events including:

* Potholes
* Construction zones
* Road obstructions
* Barricades
* Abandoned vehicles
* Debris
* Waterlogging

The system is model-agnostic and is designed to receive inference results through an API.

> **Note:** Detection classes depend on the dataset and model used for training/fine-tuning. The prototype includes a demo inference mode while the architecture remains ready for integration with a production YOLO inference service.

---

## 🔄 How Tracko Works

### Step 1 — Bus Travels

A public transport bus moves through its assigned route.

### Step 2 — Camera Observes

The onboard camera captures road conditions.

### Step 3 — AI Detects

A computer vision model analyzes video frames.

### Step 4 — Event Is Generated

The system creates an event containing:

* Detection type
* Confidence score
* Bus ID
* Timestamp
* GPS coordinates
* Image/frame reference
* Severity
* Event status

### Step 5 — Tracko Receives the Event

The centralized platform receives the event through an API.

### Step 6 — Authority Gets Actionable Intelligence

The event appears on:

* Live map
* Incident dashboard
* Alert system
* Event history
* Analytics

---

## 🖥️ Prototype

### AI Mobility Sensing

The AI dashboard demonstrates:

* Bus dashcam feed
* AI processing status
* Detection overlays
* Confidence scores
* Detection history
* Incident mapping
* AI-generated alerts
* Fleet sensor status

---

## 🛠️ Technology Stack

### Frontend

* Vite
* React
* JavaScript / TypeScript
* Responsive UI

### Backend

* REST APIs
* Event-based architecture
* Database integration

### AI / Computer Vision

* YOLO
* Computer Vision
* Video Frame Processing

### Visualization

* Interactive maps
* Mobility dashboards
* Incident analytics

### Deployment
* Vercel
* GitHub

---

## 📁 Project Structure

```text
Tracko/
├── frontend/
├── backend/
├── ai/
├── demo/
├── docs/
├── public/
├── .env.example
├── .gitignore
└── README.md
```

---

## 🚀 Running Locally

```bash
git clone <repository-url>

cd Tracko

npm install

npm run dev
```

Create a `.env` file using `.env.example` and configure the required API endpoints.

---

## 🧪 AI Demo Mode

The demonstration follows the same intended workflow:

```text
Dashcam Video
     ↓
AI Detection
     ↓
Event Generated
     ↓
Tracko API
     ↓
Map Incident
     ↓
Alert
     ↓
Analytics
```

Demo inference is clearly separated from real model inference.

---

## 🔮 Future Scope

### AI
* Custom YOLO training for Indian road conditions
* Edge AI deployment on buses
* Real-time inference
* Multi-camera fusion
* Improved detection accuracy
* Automatic severity estimation

### Mobility
* Predictive congestion analysis
* Route optimization
* Public transport demand forecasting
* Fleet health monitoring

### Smart City
* Automated authority workflows
* Incident prioritization
* Historical road-condition intelligence
* Predictive road maintenance
* City-wide sensing network

---

## 🌍 Vision
Tracko aims to create a scalable urban sensing network using infrastructure that already moves through the city every day.
**Every bus can become a sensor.
Every journey can generate intelligence.
Every detection can trigger action.**

---

## 👥 Team
Developed for **Smart India Hackathon 2026**.


## 📌 Project Status

**Prototype / SIH 2026**

The current prototype demonstrates the centralized urban intelligence platform and the AI mobility sensing workflow. The architecture is designed to support integration with a production YOLO inference service.
