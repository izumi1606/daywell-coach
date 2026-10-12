# Daywell wellness coach prototype

A single-page prototype for a voice-first wellness coach with food and calorie logging, sleep tracking, and tender document analysis.

## Run it

Open `index.html` in a modern browser. The interface can be explored in demo mode. To enable AI replies and tender summaries, choose **Connect Sarvam** and enter your Sarvam API key.

## Prototype notes

- The Sarvam key is stored in the current tab's `sessionStorage` and sent directly from the browser to Sarvam.
- The wellness metrics and meal history shown on first load are sample data.
- Tender files are read in the browser. PDFs are limited to 10 pages and need selectable text; scanned PDFs require OCR first.
- Voice input depends on browser speech recognition support. The current prototype sets English (India) as its recognition language.
- This prototype is for everyday wellness support and does not provide medical diagnosis.

## Integrations

- Sarvam Chat Completions API (`sarvam-105b-conversations`) for coaching and tender analysis.
- PDF.js for local text extraction from PDF files.
- Browser Speech Recognition and Speech Synthesis APIs for voice interaction.
