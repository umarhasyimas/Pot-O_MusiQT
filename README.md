# 🎵 Pot-O MusiQT

**Pot-O MusiQT** is a lightweight yet feature-rich desktop music player built with **Python** and **PyQt5**, designed for users who want a clean interface, strong playlist control, and practical everyday playback features without unnecessary complexity.

It focuses on **local media playback**, fast interaction, and keyboard-friendly operation, while still offering modern conveniences such as metadata handling, lyrics viewing, and smooth playback transitions.

---

## ✨ What Is Pot-O MusiQT?

Pot-O MusiQT is a **local music and media player** for Windows that supports both **audio and video files**.  
It is not a streaming client and does not require online services. Everything runs locally on your machine.

The application is built on:
- **PyQt5** for the user interface
- **Qt Multimedia (QMediaPlayer)** for playback
- **Mutagen** for metadata and cover-art handling

The goal is simple:  
> *A fast, controllable, no-nonsense music player that still feels modern.*

---

## 🚀 What You Can Expect After Installing

### 🎧 Playback Features
- Play **audio and video** files
- Smooth **Play / Pause / Stop / Next / Previous**
- Adjustable playback speed
- Volume slider with percentage display
- Resume last played track and position (state restore)

### 📂 Media & Format Support
Supported formats include:
- **Audio**: MP3, WAV, OGG, FLAC, AAC, M4A  
- **Video**: MP4, MKV, AVI, MOV, WEBM, 3GP  

> Codec availability depends on your system (Windows Media Foundation).

---

## 📑 Playlist System
- Multiple playlists using **tab-based interface**
- Drag & drop files directly into playlists
- Persistent playlists stored as JSON (auto-saved)
- Copy or move tracks between playlists
- Playlist search with debounce (responsive, non-blocking)

---

## 🏷️ Metadata & Library Tools
- Automatic metadata reading (Title, Artist, Album, Duration)
- Embedded album cover extraction
- Cover art viewer with save option
- Track **Properties dialog** (file info, codec, bitrate, duration)
- Rename files using metadata  
  *(Artist - Title.ext)*

---

## 🎼 Lyrics Viewer
- Built-in lyrics panel
- Automatic lyrics auto-scroll
- Manual scrolling supported (auto-scroll pauses when user scrolls)
- Designed to stay readable while playing

---

## ⌨️ Keyboard & Usability
- Keyboard navigation for playlist and playback
- Spacebar play/pause
- Arrow keys for navigation and track control
- Focus indicators for keyboard users
- Context menus for quick actions

---

## 🎨 Interface & Design
- Clean, modern UI with soft color palette
- Responsive layout that adapts to window size
- Album art + metadata layout inspired by classic desktop players
- Optional video panel when playing video files
- Windows taskbar integration (progress + controls)

---

## 📁 Data & Storage
Pot-O MusiQT stores its data locally:
- Playlist data:  
  `Documents/Playlist_Data/`
- Player state (last track, volume, mode):  
  `~/.player_state.json`

No telemetry. No online tracking.

---

## 🖥️ Platform
- **Windows only**
- Packaged as a standalone executable
- No Python installation required for end users

---

## 📦 Download

👉 **Download Pot-O MusiQT v1.4.2**  
[https://github.com/umarhasyimas/Pot-O_MusiQT/releases/tag/v1.4.2](https://github.com/umarhasyimas/Pot-O_MusiQT/releases/tag/v1.4.2)

---

## 📦 Installation
1. Download the latest release from the **GitHub Releases** page
2. Extract the archive
3. Run `Pot-O_MusiQT.exe`
4. Start adding your music 🎶

---

## ⚠️ Notes & Limitations
- Playback quality and supported codecs depend on installed system codecs
- This player focuses on **local files**, not streaming services
- Designed primarily for **desktop usage**, not touch-first devices

---

## 🛠️ Project Status
Pot-O MusiQT is actively developed and refined.  
The current release focuses on **stability, usability, and core playback features**.

Bug fixes and improvements are handled incrementally.

---

## 📜 License
See the repository for license details.

---

## ❤️ Credits
Developed by **Muhammad Umar Hasyim Ashari**  
Built with Python, PyQt5, and a love for classic desktop music players.

---

Enjoy your music, distraction-free.  
**Pot-O MusiQT** 🎵
