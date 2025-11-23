# Arc-AI
Arc AI is an offline-first IoT + AI system designed to enable long-range communication, smart automation, and hybrid intelligence using ESP32, LoRa, and a central hub (Raspberry Pi or computer). It continues working even without internet and seamlessly switches to cloud-based AI when connectivity becomes available.

This repository contains all the source code, circuits, documentation, and project files for the Arc AI Main Hub, Arc AI Mini Hub, and Arc AI App.

🚀 Key Features

Offline-First Architecture — Works even with zero internet.

Long-Range LoRa Communication — Multi-kilometer low-power data transmission.

Hybrid AI Engine — Uses cloud LLMs when online; local logic when offline.

Scalable IoT Network — Connect multiple ESP32 nodes to the hub.

Energy-Efficient Design — Supports battery & solar-powered mini hubs.

Cross-Platform Integration — Works with laptops, phones, and IoT nodes.

Reliable Store-and-Forward Messaging — No data loss during outages.

🧠 What Arc AI Solves

Most IoT systems break when internet connectivity is weak or unavailable. Arc AI solves this by enabling:

Communication across long distances without Wi-Fi/cell towers

Intelligent automation through cloud LLM processing

Local fallback processing when offline

Reliable remote monitoring in rural, industrial, or disaster areas

🏗️ System Architecture Overview
ESP32 Nodes <—LoRa—> Mini Hub (optional) <—LoRa—> Main Hub (Pi/Laptop) <—Internet—> Cloud AI
                                                              |
                                                           Mobile / Web App

📁 Folder Structure
Arc-AI/
│
├── arc-ai-main/        # Code & configs for main hub
├── arc-ai-mini/        # Code for mini hub / repeater
├── arc-ai-app/         # Frontend app (Next.js / React)
│   ├── package.json
│   ├── src/
│   ├── public/
│   └── .gitignore       # excludes node_modules
│
└── docs/               # Design documents & circuit diagrams


⚠️ Note: node_modules is intentionally excluded.
Install dependencies using npm install.

🔧 Setup & Installation
1. Clone the Repository
git clone https://github.com/Pranav-2310/Arc-AI.git
cd Arc-AI

2. Install App Dependencies
cd arc-ai-app
npm install

3. Run the App
npm run dev

4. Run Main Hub Scripts

Inside arc-ai-main/, run the appropriate Python/Node scripts:

python3 main_hub.py


(Adjust based on your actual file names.)

5. Mini Hub

For the mini hub:

python3 mini_hub.py

📡 Hardware Used

ESP32 Dev Boards

EBYTE E32-868T30D LoRa Modules

Raspberry Pi (Main Hub)

Solar + Battery Powered Mini Hub (optional)

Phones/Laptops for UI interaction
