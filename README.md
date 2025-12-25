# Smart Home Control Dashboard 🏠

A web-based IoT dashboard for controlling smart home devices (lights, appliances, garage doors, etc.) in real-time. Built with **HTML/JS** and **Firebase Realtime Database**, featuring secure user authentication via **Google Sign-In**.

![Project Status](https://img.shields.io/badge/status-active-success)

## 🔌 Hardware Integration (ESP32 + Relay Module)

This project is a complete **end-to-end Smart Home Automation system**, integrating a web-based dashboard with real hardware using cloud communication.

### ⚙️ System Architecture

- Smart home devices are connected to the home Wi-Fi network.
- The web dashboard communicates with **Firebase Realtime Database**.
- An **ESP32 microcontroller** is connected to the same Firebase project and listens for real-time updates.
- Appliances are controlled using **relay modules** interfaced with the ESP32.

### 🔄 Data Flow

1. User presses a control button (e.g., Light ON/OFF) on the dashboard.
2. The dashboard writes a boolean value (`true` / `false`) to Firebase Realtime Database.
3. ESP32 continuously monitors Firebase for value changes.
4. Based on the received value:
   - `true` → GPIO HIGH → Relay ON → Appliance ON  
   - `false` → GPIO LOW → Relay OFF → Appliance OFF
5. The relay physically switches the connected home appliance.


 ## link:-([https://github.com/Ankit1576734/smart_home_automatio](https://ankit1576734.github.io/smart_home_automation/))

## ✨ Features

- **🔐 Secure Authentication:** Login via Email/Password or **Google Sign-In**.
- **⚡ Real-time Control:** Toggling a switch updates the database instantly (<100ms latency).
- **📱 Responsive Design:** Works seamlessly on mobile, tablet, and desktop.
- **🔄 Live Sync:** Multiple devices stay in sync (if you turn a light on from your phone, your laptop updates instantly).
- **🎛️ Master Control:** "Turn All On" and "Turn All Off" buttons for quick management.
- **⚙️ Activity Log:** View a local history of actions performed during the session.

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3 (Tailwind CSS), Vanilla JavaScript (ES6 Modules)
- **Backend:** Firebase Realtime Database
- **Authentication:** Firebase Auth (Email & Google Provider)
- **Icons:** Heroicons (SVG)

## 🚀 Getting Started

### Prerequisites
- A Google Account (for Firebase setup)
- A code editor (VS Code recommended)
- A local server (e.g., Live Server extension for VS Code)

### Installation

1. **Clone the repository**
   ```bash
   git clone [https://github.com/Ankit1576734/smart_home_automation.git](https://github.com/Ankit1576734/smart_home_automation.git)
   cd smart_home_automation
