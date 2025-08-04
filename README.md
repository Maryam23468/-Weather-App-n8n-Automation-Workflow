# 🌦️ Weather App — n8n Workflow

A simple, automated weather update app built using [n8n](https://n8n.io/). This workflow fetches real-time weather data from the **OpenWeatherMap API** based on a user-defined city (default: Rawalpindi). It provides current temperature, humidity, wind speed, and more in a structured format.

---

## 📋 Features

- 🌍 Fetch weather for any city
- 🌡️ Current temperature and feels-like temperature
- ☁️ Weather condition and description
- 💧 Humidity level
- 💨 Wind speed
- 🔁 Easily customizable

---

## 🧠 Workflow Overview

The workflow consists of four key nodes:

| Node                      | Description                                                      |
|---------------------------|------------------------------------------------------------------|
| `Manual Trigger`          | Starts the workflow manually                                     |
| `Edit Fields`             | Sets the target city (default: Rawalpindi)                      |
| `OpenWeatherMap`          | Calls the OpenWeatherMap API to fetch live weather data         |
| `Edit Fields1`            | Formats and structures the weather data into a clean output     |

---

## 🧰 Prerequisites

- 🛠️ [n8n](https://n8n.io/) instance (cloud or self-hosted)
- 🔑 OpenWeatherMap API key ([Get one here](https://openweathermap.org/api))

---

## ⚙️ Setup Instructions

1. **Clone or Import** this workflow JSON into your n8n instance.
2. **Create Credentials**:
   - Go to **Credentials** tab in n8n
   - Create a new credential for **OpenWeatherMap**
   - Paste your API key and name it `OpenWeatherMap account`
3. **Set Your City**:
   - Open the `Edit Fields` node
   - Change `"Rawalpindi"` to your desired city

---

## 🚀 How to Use

1. Open your n8n instance
2. Open this workflow
3. Click on **“Execute Workflow”**
4. You will receive an output like this:

```json
{
  "Location": "Rawalpindi",
  "Temperature": "33°C",
  "Feels like": "36°C",
  "Weather": "Clouds (scattered clouds)",
  "Humidity": "55%",
  "WindSpeed": "4.6 m/s"
}
