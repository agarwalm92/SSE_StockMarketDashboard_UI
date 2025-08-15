# Real-Time Stock Price Dashboard (SSE UI)

## Overview
This repository contains a simple frontend dashboard that consumes the **Server-Sent Events (SSE)** API and displays live stock price updates with visual cues for price changes.

---

## Features
- Connects to an SSE backend and receives real-time updates.
- Color-coded stock movement:
  - Green = Price increased
  - Red = Price decreased
- Automatically updates without manual refresh or polling.
- Responsive, minimal UI for quick data visualization.

---

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Protocol:** Server-Sent Events (HTTP)
- **Data Source:** Real-Time Stock Price API

---

## How It Works
1. The dashboard connects to the API’s SSE endpoint using `EventSource`.
2. Incoming JSON messages are parsed and displayed instantly.
3. Stocks update every few seconds with a visual color indicator for changes.

---

## Use Cases
This approach is ideal for:
- Live financial dashboards
- Sports scoreboards
- Real-time order tracking
- System health monitoring

---

## Advantages
- No WebSocket complexity — works out of the box in modern browsers.
- Automatic reconnection handled by the browser.
- Low latency and reduced server load compared to polling.

---

## Related Article
For the step-by-step tutorial on setting up the API and UI, see:  
[Implementing Real-Time Updates with SSE in C# .NET — A Complete Guide](https://dev.to/mayank_agarwal/implementing-real-time-updates-with-server-sent-events-sse-in-c-net-a-complete-guide-248l)

---

## License
This project is licensed under the MIT License.
