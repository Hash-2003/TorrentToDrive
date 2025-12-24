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
1. Open notebook in Google Colab
2. Mount Google Drive
3. Execute cells sequentially
4. Interrupt and resume to observe reliability behavior
