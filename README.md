# 🌾 Agri-Sheild

<div align="center">

![Agri-Sheild Logo](https://img.shields.io/badge/🌾-Agri--Sheild-green?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMTMuMDkgOC4yNkwyMCA5TDEzLjA5IDE1Ljc0TDEyIDIyTDEwLjkxIDE1Ljc0TDQgOUwxMC45MSA4LjI2TDEyIDJaIiBmaWxsPSIjNjZCQjZBIi8+Cjwvc3ZnPgo=)

**Smart Agriculture Solution for Crop Protection & Environmental Monitoring**

[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-2.0+-red?style=flat-square&logo=flask)](https://flask.palletsprojects.com)
[![IoT](https://img.shields.io/badge/IoT-Enabled-green?style=flat-square&logo=internetofthings)](https://github.com/Harsha-o3/Agri-Sheild)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/Harsha-o3/Agri-Sheild?style=flat-square)](https://github.com/Harsha-o3/Agri-Sheild/stargazers)

[🚀 Demo](#-demo) • [📥 Installation](#-installation) • [📖 Documentation](#-documentation) • [🤝 Contributing](#-contributing)

</div>

---

## 🌟 Overview

**Agri-Sheild** is a cutting-edge smart agriculture solution that revolutionizes crop protection and environmental monitoring. By seamlessly integrating IoT sensors with a powerful web-based dashboard, it empowers farmers with real-time insights and intelligent alerts to make data-driven decisions and maximize agricultural productivity.

### 🎯 Problem Statement
Modern agriculture faces challenges including:
- ❌ Unpredictable weather patterns
- ❌ Inefficient resource management  
- ❌ Delayed response to environmental threats
- ❌ Limited real-time monitoring capabilities

### 💡 Our Solution
Agri-Sheild provides a comprehensive monitoring system that:
- ✅ Delivers real-time environmental data
- ✅ Sends proactive alerts for optimal crop protection
- ✅ Enables remote monitoring via web dashboard
- ✅ Supports data-driven agricultural decisions

---

## ✨ Key Features

<table>
<tr>
<td width="50%">

### 🌡️ **Real-Time Monitoring**
- Temperature & humidity tracking
- Soil moisture analysis
- Light intensity measurement
- Air quality assessment

### 🔔 **Intelligent Alerts**
- Customizable threshold notifications
- SMS/Email alert integration
- Weather-based risk assessment
- Automated irrigation triggers

</td>
<td width="50%">

### 📊 **Real-Time Monitoring**
- Temperature & humidity tracking
- Soil moisture analysis
- Light intensity measurement
- Environmental data logging

### 🌐 **User-Friendly Interface**
- Responsive web dashboard
- Mobile-optimized design
- Real-time data updates
- Intuitive control panels

</td>
</tr>
</table>

---

## 🛠️ Technology Stack

<div align="center">

| Category | Technologies |
|----------|-------------|
| **Backend** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white) |
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| **Hardware** | ![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberry-pi&logoColor=white) |
| **Sensors** | DHT11/22, Soil Moisture, Light Sensors, pH Sensors |

</div>

---

## 🚀 Quick Start

### 📋 Prerequisites

Before you begin, ensure you have the following installed:

```bash
✅ Python 3.8 or higher
✅ Git
✅ Hardware sensors (DHT11, Soil Moisture, etc.)
✅ Arduino IDE (for microcontroller programming)
```

### 📥 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Harsha-o3/Agri-Sheild.git
   cd Agri-Sheild
   ```

2. **Set up virtual environment** (recommended)
   ```bash
   python -m venv agri_env
   source agri_env/bin/activate  # On Windows: agri_env\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure sensors** (optional)
   ```bash
   # Edit config.py to match your sensor setup
   nano config.py
   ```

5. **Launch the application**
   ```bash
   python app.py
   ```

6. **Access the dashboard**
   ```
   🌐 Open your browser and navigate to: http://localhost:5000
   ```

---

## 📱 Demo

<div align="center">

### 🖥️ Dashboard Overview
![Dashboard](Flask/static/images/4.jpg)

### 📊 Monitoring Interface
![Monitoring Interface](Flask/static/images/b2.jpg)

### 🔔 System Controls
![System Controls](Flask/static/images/b3.jpg)

### 📈 Application Interface
![Application Interface](Flask/static/images/b7.jpg)

</div>

---

## 📁 Project Structure

```
Agri-Sheild/
├── 📁 Flask/                 # Flask application files
├── 📁 Src/                   # Source code
├── 📁 test_images/           # Test images and assets
├── 📄 .gitignore            # Git ignore rules
├── 📄 README.md             # Project documentation
├── 📄 package.json          # Node.js dependencies
├── 📄 requirements.txt      # Python dependencies
└── 📄 app.py               # Main application entry point
```

---

## 🌟 Usage Examples

### 🔧 Basic Sensor Integration

```python
# Example: Reading sensor data
from sensors import DHT22Sensor, SoilMoistureSensor

# Initialize sensors
temp_sensor = DHT22Sensor(pin=2)
moisture_sensor = SoilMoistureSensor(pin=A0)

# Read data
temperature = temp_sensor.read_temperature()
humidity = temp_sensor.read_humidity()
soil_moisture = moisture_sensor.read_moisture()

print(f"Temperature: {temperature}°C")
print(f"Humidity: {humidity}%")
print(f"Soil Moisture: {soil_moisture}%")
```

### 🔔 Setting Up Alerts

```python
# Example: Configure alert thresholds
alert_config = {
    'temperature': {'min': 15, 'max': 35},
    'humidity': {'min': 40, 'max': 80},
    'soil_moisture': {'min': 30, 'max': 70}
}
```

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### 🚀 How to Contribute

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### 🐛 Bug Reports

Found a bug? Please create an issue with:
- Bug description
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)

### 💡 Feature Requests

Have an idea? We'd love to hear it! Open an issue with:
- Feature description
- Use case scenario
- Proposed implementation (optional)

---

## 📊 Project Stats

<div align="center">

![GitHub contributors](https://img.shields.io/github/contributors/Harsha-o3/Agri-Sheild?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/Harsha-o3/Agri-Sheild?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/Harsha-o3/Agri-Sheild?style=flat-square)
![GitHub pull requests](https://img.shields.io/github/issues-pr/Harsha-o3/Agri-Sheild?style=flat-square)

</div>

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

<div align="center">

**Anuhya Avadhanam**

*"Innovating agriculture through technology, one sensor at a time."*

</div>

---

## 🙏 Acknowledgments

- Thanks to all contributors who have helped shape this project
- Inspired by the need for sustainable and smart farming solutions
- Special thanks to the open-source community for the amazing tools and libraries

---

<div align="center">

### ⭐ Don't forget to star this repository if you found it helpful!

**Made with ❤️ for farmers and agriculture enthusiasts worldwide**

</div>
