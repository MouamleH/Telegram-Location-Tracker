# Telegram Location Tracker

A minimalistic location tracking bot for Telegram with real-time web visualization. <br>
A different take on [MouamleH/tg-live-location-bot](https://github.com/MouamleH/tg-live-location-bot)

## What it does

- 📍 Tracks user locations shared via Telegram
- 🗺️ Displays locations on an interactive web map
- 📱 Sends messages back to users through the web interface
- 🛣️ Shows user movement paths with road routing
- ⚡ Real-time updates using WebSocket connections

## Tech Stack

- **Backend**: Go with PocketBase (embedded database + real-time API)
- **Frontend**: Vanilla JavaScript with Alpine.js and Leaflet maps
- **Bot**: Telegram Bot API integration
- **Database**: SQLite (via PocketBase)

## Quick Start

1. Set up your environment:
   ```bash
   mv .env.example .env
   # Add your BOT_TOKEN from @BotFather
   ```

2. Run the application:
   ```bash
   go run main.go
   ```

3. Open `http://localhost:8080` to view the map interface

## Features

- **Smart filtering**: Only saves locations when users move >10 meters (reduces GPS noise)
- **Clustering**: Groups nearby users on the map
- **Path visualization**: Toggle to show user movement history
- **Two-way communication**: Send messages to users directly from the web interface
- **Real-time updates**: See location changes instantly

---

*This project was vibe coded* ✨
