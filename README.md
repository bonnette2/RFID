# 💳 Emerald Wallet | RFID Top-Up Ecosystem

Emerald Wallet is a high-performance RFID card top-up ecosystem that combines an ESP8266 edge device, a Node.js backend bridge, and a real-time web dashboard.  
The system supports secure RFID balance storage, real-time monitoring, and remote top-up operations using MQTT, HTTP, and WebSockets.

---

# 🌍 Live Web Dashboard

**Public Dashboard URL:**

http://157.173.101.159:9273/wallet.html

This dashboard provides real-time card detection, balance display, and top-up controls.

---

# 🧱 System Architecture

The system uses a 3-layer architecture:

## 1️⃣ Edge Layer — ESP8266 Emerald Hub
- Reads RFID cards using MFRC522
- Stores balance on the card (Sector 2, Block 8)
- Connects to WiFi network
- Publishes and receives messages via MQTT
- Uses isolated topic namespace:

