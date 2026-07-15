# Tank Level Monitoring System (IoT Simulation)

## Problem Statement
Monitoring level tangki secara manual di lapangan rawan human error dan
delay deteksi kondisi kritis (level terlalu rendah/tinggi). Project ini
mensimulasikan sistem monitoring real-time berbasis IoT.

## Tech Stack
- ESP32 (simulasi via Wokwi) + sensor ultrasonic HC-SR04
- Protokol MQTT (HiveMQ public broker)
- Node-RED sebagai middleware & dashboard
- (Next: InfluxDB + Grafana untuk historical data & OEE-style reporting)

## Architecture
[diagram di sini]

## Demo
![demo](assets/demo.gif)
Live simulation: [link Wokwi project]

## How to Run
1. Buka link Wokwi, klik Run
2. Import `node-red-flow/flow.json` ke Node-RED
3. Deploy, buka http://localhost:1880/ui

## Future Improvements
- Ganti broker publik dengan private/self-hosted (security)
- Tambah multi-tank monitoring
- Integrasi historical data storage (InfluxDB) + Grafana dashboard
- Tambah notifikasi ke Telegram/WhatsApp saat alarm