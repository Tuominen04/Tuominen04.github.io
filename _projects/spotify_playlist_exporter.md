---
layout: page
title: Spotify Playlist Exporter
description: A simple Python script to export song titles and artists from a Spotify playlist into a CSV file.
img: assets/img/spotify_project/spotify_banner.jpg
importance: 2
category: fun
related_publications: true
---

---

<br/>

### 🎶 Spotify Playlist Exporter  

This project is a small Python script that connects to the **Spotify Web API** and exports the songs from any public Spotify playlist into a neat **CSV file**.  
It’s useful if you want to back up playlists, analyze your music, or just keep a record of your favorite tracks outside Spotify.  

<br/>

### ✨ Features
- Export all tracks from a public playlist
- Saves track **title** and **artist(s)** into `track_info.csv`
- Supports playlists of any length (pagination included)
- Easy setup with a `.env` file (no secrets in the code)

<br/>

### 🚀 How It Works
1. Authenticate with Spotify using your own **Client ID** and **Secret**  
2. Provide a playlist link in the `.env` file  
3. Run the script → get a `CSV` with all tracks and artists  

<br/>

### 📂 Repository
🔗 [View on GitHub](https://github.com/Tuominen04/spotify-playlist-exporter)

<br/>

### 🛠️ Tech Stack
- Python  
- [Spotipy](https://spotipy.readthedocs.io/en/2.24.0/) (Spotify Web API wrapper)  
- dotenv for environment management

<br/>

### 📸 Screenshots
<div class="row justify-content-left text-center">
    <div class="col-md-5 mb-3">
        {% include figure.liquid path="assets/img/spotify_project/track_info_csv.png" 
           title="Real-life setup" class="img-fluid rounded z-depth-2" %}
        <p class="small text-muted mt-2">Example image of .csv file</p>
    </div>
</div>

<br/>