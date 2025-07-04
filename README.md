# 🛡️ Media Automation Stack with VPN

This repository defines a Docker-based media automation stack where all applications route traffic securely through NordVPN using Gluetun. The stack automates downloading, organizing, and streaming media while ensuring privacy.

## ✨ Features

- **Secure VPN routing**
  - All download and indexer traffic routed through NordVPN via Gluetun
  - Built-in firewall and killswitch — no leaks

- **Automated media management**
  - 📥 **qBittorrent** — Torrent client for downloading
  - 🎬 **Radarr** — Movies (auto-search, download, organize)
  - 📺 **Sonarr** — TV series (auto-download, organize)
  - 🎵 **Lidarr** — Music (artist/album tracking, downloads)
  - 📚 **Readarr** — eBooks and audiobooks management
  - 🌐 **Prowlarr** — Unified indexer management for all apps
  - 📝 **Bazarr** — Subtitle downloading and syncing

- **Media servers**
  - 🎥 **Plex** — Media server for streaming anywhere
  - 📺 **Jellyfin** — Open-source media streaming

- **Local LAN access (todo)**
  - Ports exposed for local network access
  - Can be combined with a reverse proxy (e.g. Nginx Proxy Manager) for external HTTPS access

## 🛠 Stack Components

| Service     | Purpose                        |
|-------------|--------------------------------|
| Gluetun     | VPN tunnel + firewall (NordVPN) |
| qBittorrent | Torrent client                  |
| Radarr      | Movie management                |
| Sonarr      | TV series management            |
| Lidarr      | Music management                |
| Readarr     | Book management                 |
| Prowlarr    | Indexer manager                 |
| Bazarr      | Subtitle automation             |
| Plex        | Media streaming (Plex.tv)       |
| Jellyfin    | Open-source media streaming     |

## 🚀 Deployment

Run the stack:
```bash
docker-compose up -d
