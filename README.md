# Reliable Data Ingestion in Ephemeral Environments (Google Colab)

## Overview
This project demonstrates how to design a restart-safe, integrity-verified
data ingestion pipeline in an ephemeral compute environment using Google Colab
and Google Drive.

A legally distributed Ubuntu LTS ISO is used as the example artifact.

## Key Concepts
- Ephemeral compute vs persistent storage
- Resume-safe downloads
- Integrity verification
- Idempotent pipeline design
- Logging and observability

## Why BitTorrent?
BitTorrent is used purely as a transport protocol due to:
- Built-in chunk verification
- Resume capability
- Distributed availability

No copyrighted or unauthorized content is involved.

## Architecture
Colab Runtime → Torrent Client → Google Drive (Persistent Storage)

## How to Run

1. **Download the repository**
   - Clone or download this repository to your local machine.

2. **Upload the notebook to Google Drive**
   - Upload `TorrentToDrive.ipynb` to any folder in your Google Drive.

3. **Open the notebook in Google Colab**
   - Right-click the notebook in Google Drive → *Open with* → *Google Colab*.

4. **Mount Google Drive**
   - Run the first cell to mount Google Drive.
   - This enables persistent storage and resumable execution across Colab restarts.

5. **Configure the torrent source**
   - Set the `TORRENT_LINK` variable to a **legally distributed `.torrent` file**
     (for example, an official Linux distribution torrent).

6. **Connect the runtime**
   - Ensure the Colab runtime is connected (CPU runtime is sufficient).

7. **Run the pipeline**
   - Select **Runtime → Run all**.
   - The download will start automatically.
   - If the runtime disconnects, re-running the notebook will resume from where it stopped.

---

## Notes
- This project is intended for **educational purposes only**.
- Only **legally distributed torrents** should be used.
- Large binary files, logs, and session state are excluded from version control.
- Torrent connectivity may vary depending on Colab’s network restrictions.

---
