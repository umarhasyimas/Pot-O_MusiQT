# Pot-O MusiQT

**Lightweight Free Audio Player** for Windows

**Latest version: v2.8.2 — "Verse"**

Pot-O MusiQT is a fast, controllable, no-nonsense music player that still feels modern. It plays your own local music library with gapless playback, crossfade, a graphic equalizer, a live spectrum visualizer, a lyrics panel and customizable color themes. It has no streaming, no accounts and no telemetry. Everything stays on your computer.

[Website](https://musiqt.pages.dev) · [Download (Releases)](https://github.com/umarhasyimas/Pot-O_MusiQT/releases)

---

## Download and install

1. Open the [Releases](https://github.com/umarhasyimas/Pot-O_MusiQT/releases) page and download the installer for your Windows edition:
   - `PotOMusiQT_Setup_2.8.2_x64.exe` — 64-bit Windows (recommended)
   - `PotOMusiQT_Setup_2.8.2_x86.exe` — 32-bit edition
2. Run the installer. It lets you choose the install folder, create a desktop shortcut, make Pot-O MusiQT your default music player, and reset preferences left by an earlier install. A previous version is detected and replaced automatically.
3. Start Pot-O MusiQT from the Start menu or the desktop shortcut.

The installer needs administrator rights only to install. **The player itself runs as a normal user and never asks for administrator rights**, because everything it saves goes to your own user profile.

Older releases (such as v1.x) remain available on the Releases page.

**Requirements:** Windows 10 or newer · a sound device · about 200 MB of disk space. No Python, Qt or codec pack is needed. Everything is bundled.

---

## Features

### Playback
- Play / pause / stop / next / previous, seeking and volume
- **Gapless playback** and **crossfade** between tracks
- Shuffle and repeat (off / all / one), plus **A-B repeat** for a section of a track
- **Playback speed** and **pitch control**
- **ReplayGain / volume normalization**, so tracks of different loudness play at a similar level
- **Sleep timer**
- Choose the **output device**, mono / stereo output and channel mapping
- Resumes your last track and position on start

### Sound
- **8-band graphic equalizer** with built-in presets and a *Custom* preset that is selected automatically when you move a slider
- Save, load and reset your own EQ presets
- **Auto EQ**: picks a preset from the track's Genre tag (spoken-word genres such as Quran recitation, podcasts and audiobooks stay flat)
- Balance and pre-amp controls

### Library and playlists
- Multiple **playlist tabs**
- **Favorites**: click the star on any track; all favorites appear in the ★ Favorites tab
- Open files, a folder, a folder with subfolders, a disc, or **ZIP archives** (including password-protected ones)
- **Watch folders**: keep a playlist in sync with a folder automatically
- Copy or move tracks between playlists, drag to reorder, and sort
- **Undo / redo** for playlist edits
- Quick search inside a playlist, and *Jump to Playing*
- Save and load playlists as **M3U**, and export playlist data as **CSV** or **JSON**
- Expand the playlist to see a file-info line under every track (format, sample rate, bitrate, channels, file size)

### Metadata, cover art and lyrics
- Reads title, artist, album, duration and cover art
- **Edit tags**, embed cover art and lyrics, and save cover art to a file
- Rename files from their metadata
- Lyrics panel with adjustable text size and a full-height expand mode

### Look and feel
- **Live spectrum visualizer**
- **Color themes**, including *Amber Glow*, *Coral Dusk* and *Sunset*
- **Your own themes**: *Color Theme → Export theme template*, edit the colors, then *Import custom theme*. Imported themes are kept in your user profile and are there every time you start the player
- Full window and compact (mini player) modes
- Windows taskbar integration
- Double-click a song in Explorer to play it. If Pot-O MusiQT is already running, the song is handed to that window

### Your settings
- **Export / import settings** for backup
- **Reset All Preferences (Factory Reset)** that keeps your playlists and music files

---

## Supported audio formats

MP3 · FLAC · WAV · OGG · Opus · M4A · AAC · WMA · WebM (audio only)

Video playback was removed in the 2.x series. Pot-O MusiQT is an audio player.

---

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / Pause |
| `Right` | Next track |
| `Alt` + `Right` | Next track (when focused on the playlist) |
| `Left` | Previous track |
| `Ctrl` + `O` | Open files… |
| `Ctrl` + `Shift` + `O` | Open folder… |
| `Ctrl` + `D` | Open disc… |
| `Ctrl` + `F` | Search |
| `Ctrl` + `E` | Edit metadata |
| `Home` | Jump to playing track |
| `Ctrl` + `Z` | Undo playlist edit |
| `Ctrl` + `Shift` + `Z` or `Ctrl` + `Y` | Redo playlist edit |
| `Ctrl` + `S` | Save state |
| `Alt` + `X` | Quit |

---

## Where your data is stored

Everything is stored per user in `%APPDATA%\PotOMusiQT`:

| Item | Location |
| --- | --- |
| Playlists | `playlists\playlists.db` |
| Settings and player state | `state.json`, `watch_folders.json`, `favorites.json` |
| Your imported color themes | `themes\` |
| Log file | `logs\PotOMusiQT.log` (useful when reporting a problem) |

Your music files are never moved, changed or deleted by the installer or uninstaller. Tag editing changes only the files you choose to edit.

---

## Uninstall

*Settings → Apps → Installed apps → Pot-O MusiQT → Uninstall.* The uninstaller restores the file associations that existed before and asks whether you also want to delete your settings, favorites and saved playlists.

---

## Status

Actively developed. Bug reports and feature ideas are welcome through the [Issues](https://github.com/umarhasyimas/Pot-O_MusiQT/issues) page. Please attach `logs\PotOMusiQT.log` when reporting a problem.

---

## License

Pot-O MusiQT is distributed as a **compiled binary only** under the *Pot-O MusiQT Binary License*:

- Free for personal and private use
- You may redistribute the original, unmodified binary package
- No reverse engineering, modification, derivative works or commercial redistribution without permission
- Provided "as is", without warranty

The full text is shown in the installer and in the app under *About → License*. For permissions beyond this license, please contact the author at [umarhasyimas@gmail.com](mailto:umarhasyimas@gmail.com).

Copyright © 2026 Muhammad Umar Hasyim Ashari. All rights reserved.

---

## Credits

Created by **Muhammad Umar Hasyim Ashari** — owner, programmer and designer. Logo & icons designed by Muhammad Umar Hasyim Ashari. 

Built with these third-party components, each used under its own license:

| Component | Used for | License |
| --- | --- | --- |
| [Python](https://www.python.org) 3.13 | Programming language | PSF License |
| [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) | User interface bindings | GPL v3 or Riverbank Commercial License |
| [Qt 5](https://www.qt.io) | Application framework | LGPL v3 / GPL v3 / Commercial |
| [BASS](https://www.un4seen.com) and add-ons | Audio engine and format decoders | Free for non-commercial use; commercial use requires a license from Un4seen Developments |
| [mutagen](https://mutagen.readthedocs.io) | Reading and writing tags | GPL v2 or later |
| [NumPy](https://numpy.org) | Numerical computing | BSD 3-Clause |
| [SQLite](https://www.sqlite.org) | Playlist database | Public Domain |
| [OpenSSL](https://www.openssl.org) | Cryptography libraries bundled with Python and Qt | Apache 2.0 (3.x) / OpenSSL and SSLeay (1.1.x) |

All trademarks and copyrights belong to their respective owners.
