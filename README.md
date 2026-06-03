# GeoInt Bug Bounty Toolkit

**AI-powered geolocation and OSINT tool for bug hunters and security researchers.**

## 🎯 Purpose

This toolkit helps ethical bug bounty hunters and penetration testers discover physical location intelligence from images. It combines:

- **AI‑based geolocation** (similar to GeoSpy) – analyse landscapes, architecture, signs, vegetation to pinpoint coordinates.
- **EXIF & metadata extraction** – GPS, timestamps, camera models.
- **Reverse image search** – find similar images across the web.
- **OpenStreetMap / Google Maps integration** – visualise and refine results.

The goal is to assist in authorised security assessments where physical infrastructure (e.g., server rooms, office buildings, data centres) appears in leaked or public images.

## 🚀 Features

| Feature | Description |
|---------|-------------|
| 🔍 **AI Geolocation** | Uses fine‑tuned Vision‑Language Models (LLaVA, MiniCPM‑V, GeoCLIP) to estimate latitude/longitude from a single photo. |
| 📍 **Chain‑of‑Thought reasoning** | Explains *why* a location was chosen (e.g., “Soviet panel buildings + birch trees + Cyrillic sign → likely Russia”). |
| 🧩 **Metadata parser** | Extracts GPS, timestamps, and camera settings from EXIF. |
| 🗺️ **Map refinement** | Overlays predictions on OpenStreetMap or Google Maps for manual verification. |
| 🐞 **Bug hunting workflows** | Example playbooks: find a server’s city from a random photo of a rack, or identify a company’s physical address from a leaked cafeteria picture. |
| 🤖 **Local & private** | Everything runs on your machine or your own cloud – no third‑party API for image upload. |

## 🛠️ Installation

```bash
git clone https://github.com/bumahkib7/geoint-bagbounty-toolkit.git
cd geoint-bagbounty-toolkit
pip install -r requirements.txt
