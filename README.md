# IP-TRACKER-CYBER-TOOL
 IP Activity Tracker is a Python-based desktop tool for analyzing public IPv4/IPv6 addresses. It provides IP validation, geolocation and network metadata, threat scoring, activity classification, map integration, live monitoring, lookup history, auto-refresh, report export, and light/dark themes.
# 🔍 IP Activity Tracker

A practical Python-based desktop application for analyzing **public IPv4 and IPv6 addresses**. The tool retrieves geolocation and network information from public APIs, classifies likely network activity, calculates a threat score, and provides useful reporting and monitoring features.

> **Note:** This project provides public IP intelligence and approximate geolocation data. It does not track a person in real time and should only be used for legitimate network, security, and technical investigations.

---

## 🚀 Features

* ✅ IPv4 and IPv6 address validation
* 🌍 IP geolocation information
* 🌐 Network and ISP information
* 🏢 ASN and organization details
* 📡 Network type detection
* 🛡️ VPN / Proxy / Tor detection
* ☁️ Cloud and hosting detection
* ⚠️ Threat score from 0–100
* 🔎 Threat level classification
* 🗺️ Open IP location in Google Maps
* 📊 Activity and risk classification
* 🔄 Auto-refresh functionality
* 👁️ Live IP monitoring
* 📝 Lookup history
* 📋 Copy reports to clipboard
* 📄 Export reports as `.txt`
* 📸 Save application snapshots
* 🌙 Light and dark mode
* 💻 Desktop GUI using Tkinter

---

## 🛠️ Technologies Used

* **Python**
* **Tkinter** – Desktop graphical user interface
* **Requests** – API requests
* **JSON** – Data storage and processing
* **RDAP** – IP registration/network information
* **ipaddress** – IP validation
* **Google Maps** – Location visualization
* **Pillow** – Application snapshot functionality

---

## 🌐 Data Sources

The application uses public services to retrieve IP information, including:

* `ipapi.co`
* `ipinfo.io`
* `ip-api.com`
* RIPE RDAP
* RDAP.org

The application attempts multiple public API sources and normalizes their responses into a common format.

---

## 📊 Information Provided

For a valid public IP address, the application can display information such as:

* IP Address
* Country
* Region
* City
* Postal Code
* Timezone
* Latitude
* Longitude
* Organization / ISP
* ASN
* Hostname
* Network Type
* Threat Score
* Threat Level
* Activity / Risk Profile
* WHOIS / RDAP information
* Google Maps location

---

## ⚠️ Threat Scoring

The application calculates a score between **0 and 100** using available metadata.

Threat levels are classified as:

| Score  | Level    |
| ------ | -------- |
| 0–29   | Low      |
| 30–49  | Medium   |
| 50–74  | High     |
| 75–100 | Critical |

The score is based on factors such as proxy/VPN/Tor indicators, hosting infrastructure, mobile networks, missing location information, threat metadata, and organization keywords.

**Important:** The threat score is a heuristic created by this project and should not be treated as a definitive security verdict.

---

## 📁 Project Structure

```text
IP-Activity-Tracker/
│
├── IP ACTIVITY TRACKER(1).py
├── ip_activity_history.json
└── README.md
```

Report and snapshot files can also be generated while using the application.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### 2. Enter the project directory

```bash
cd YOUR-REPOSITORY
```

### 3. Install the required Python package

```bash
pip install requests
```

For snapshot functionality, install Pillow:

```bash
pip install Pillow
```

---

## ▶️ Run the Application

Run the Python file:

```bash
python "IP ACTIVITY TRACKER(1).py"
```

The application will open as a desktop GUI.

Enter a public IPv4 or IPv6 address and click **Track IP**.

---

## 🔎 Example

You can test the application with a public IP such as:

```text
8.8.8.8
```

The application will attempt to retrieve available network and geographic information and display the generated report.

---

## 📌 Main Functions

### Track IP

Analyzes the entered public IP address and retrieves available metadata.

### My Public IP

Attempts to determine the machine's current public IP.

### Open Map

Opens the estimated IP location in Google Maps.

### Live Monitor

Allows IP addresses to be added to a monitoring list and refreshed periodically.

### Auto Refresh

Automatically performs repeated IP lookups at a specified interval.

### History

Stores recent lookup results locally for later viewing.

### Export Report

Exports the current IP analysis as a text report.

### Save Snapshot

Attempts to save a screenshot of the application using Pillow.

---

## 🔐 Privacy & Responsible Use

This project is intended for:

* Network learning
* Cybersecurity education
* IP analysis
* Technical investigations
* Network administration
* Personal projects

It should **not** be used to stalk, harass, identify, or monitor people without authorization.

IP geolocation is approximate and does not necessarily represent the physical location of a specific person or device.

---

## 🧑‍💻 Proje
