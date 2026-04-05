# Valiutos – Currency Exchange Rate Viewer

An Android app that fetches and displays live currency exchange rates
from the European Central Bank (ECB).

## Features
- Fetches real-time EUR exchange rates from the official ECB API
- Parses XML response data
- Displays all currencies in a scrollable list
- Live search/filter to quickly find a specific currency
- Async network requests (AsyncTask) to keep UI responsive

## Tech Stack
- Java
- Android SDK
- ECB XML API (`eurofxref-daily.xml`)
- XML parsing via DOM (DocumentBuilder)
- Gradle (Kotlin DSL)

## Architecture
- `MainActivity` – UI, filter logic, list display
- `DataLoader` – async HTTP request (AsyncTask + callback interface)
- `Parser` – XML DOM parser, extracts currency/rate pairs

## Data Source
European Central Bank:
https://www.ecb.europa.eu/stats/eurofxref/eurofxref-daily.xml

## How to run
1. Clone the repo
2. Open in Android Studio
3. Make sure device/emulator has internet access
4. Run on emulator or physical device

## Notes
Built at Vilnius University (2024).
Covers: AsyncTask, HTTP networking, XML DOM parsing,
TextWatcher filtering, callback interfaces.
