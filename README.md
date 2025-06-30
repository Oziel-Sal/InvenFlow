# 📦 InvenFlow

**InvenFlow** is an AI-powered smart inventory management system designed for cafés, restaurants, and small businesses. It combines real-time sensor data, machine learning, and optional computer vision to monitor inventory levels, forecast usage, and help automate restocking.

![Dashboard Preview](./assets/dashboard_preview.png)

---

## 🚀 Features

* 📊 **Real-time inventory tracking** using weight sensors and optional cameras
* 🧠 **AI-powered forecasting** to predict usage and run-out dates
* 🛐 **Smart alerts** for low stock or expiring items
* 📈 **Weekly trends dashboard** for cost and quantity visualization
* 🛠️ **Modular setup** for items like coffee beans, cups, milk, and pastries
* 🌐 **Touch-friendly UI** for staff interaction on tablets or kiosk screens

---

## 📦 Use Case Example

* Coffee beans tracked by load cells
* Milk monitored by weight and temperature sensors
* Cups and lids counted using IR or load sensors
* Pastries logged and forecasted by daily weight drop
* AI model predicts daily consumption and triggers alerts when thresholds are reached

---

## 🛠️ Tech Stack

| Category        | Tools                                 |
| --------------- | ------------------------------------- |
| Programming     | Python                                |
| AI/ML           | scikit-learn, joblib, Pandas          |
| Sensor Hardware | Raspberry Pi 4, HX711, Load Cells     |
| Optional Vision | OpenCV, Pi Camera Module              |
| Dashboard       | Flask or Streamlit                    |
| Data Storage    | SQLite / Firebase / Google Sheets API |

---

## 📁 Project Structure

```bash
invenflow/
│
├── sensors/         # Weight, temp, IR, and camera integrations
├── ai/              # Machine learning models (train, predict)
├── dashboard/       # Streamlit or Flask frontend
├── data/            # Local data logs (CSV, DB)
├── utils/           # Helpers, graphing, I/O functions
├── assets/          # UI images, mockups, icons
├── README.md        # This file
└── requirements.txt # Dependency list
```

---

## ⚙️ Getting Started

### 🔧 Requirements

* Raspberry Pi 4 (or ESP32)
* Load Cell + HX711 module
* Python 3.8+
* Basic electronics knowledge (for wiring sensors)

### 🐍 Install Python Packages

```bash
pip install -r requirements.txt
```

### 🚀 Run the App

```bash
python inventory_ai.py         # logs weight and trains model
streamlit run dashboard/app.py # launches the inventory UI
```

---

## 📈 Dashboard Snapshot

![Graph Example](./assets/forecast_widget.png)

---

## 🧠 AI Forecasting

* Uses linear regression (scikit-learn) to estimate daily usage
* Predicts run-out date for each item based on trends
* Optionally plots forecast vs. historical data
* Can extend to Prophet or LSTM for more advanced models

---

## 🛡️ License

MIT License. Feel free to use, fork, and improve this system.

---

## 🙌 Contributors

* Oziel Salinas – Founder / Developer
* ChatGPT – Technical planning and AI guidance

---

## 📬 Contact

Want to collaborate or use this in your café?
Email: \[[your\_email@example.com](mailto:your_email@example.com)]
LinkedIn: \[your LinkedIn link]
Website: \[your brand or coffee shop site]

---

> Built for small businesses with big ideas.
