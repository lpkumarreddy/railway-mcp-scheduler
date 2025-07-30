---

## 📘 Project Guide: Railway Train Schedule – Hyderabad to Tirupati (Project-3)

### 🚀 Overview

This project demonstrates how to use **Cursor IDE** with an integrated **MCP+LLMs server** to retrieve real-time Indian Railway data using natural language prompts. The focus is on trains between **Hyderabad and Tirupati**, including schedules, seat availability, and live train status.

---

### 🛠️ Requirements

* Cursor IDE (v1.3.5 or higher)
* MCP+LLMs server (Indian Railways endpoint)
* Internet access

---

### ⚙️ MCP Server Configuration

Set up the MCP server in Cursor IDE using the following configuration:

```json
{
  "mcpServers": {
    "Indian Railway": {
      "url": "https://railway-mcp.amithv.xyz/mcp"
    }
  }
}
```

Paste this into the **MCP configuration tab** in Cursor.

---

### 🧭 Workflow

#### ✅ Step 1: Open Cursor IDE and Navigate to MCP Tab

* Open Cursor IDE
* Go to **MCP** tab
* Ensure your configuration is active and saved

#### ✅ Step 2: Use Natural Language Prompts

Use prompts like:

```
Give me the Hyderabad to Tirupati scheduled trains list on 2025-07-31.
```

---

### 🧪 Use Cases & Prompts

| Use Case                | Example Prompt                                                 |
| ----------------------- | -------------------------------------------------------------- |
| Get Train Schedule      | Hyderabad to Tirupati scheduled trains list on 2025-07-31      |
| Get Train Info          | get the train info: KRISHNA EXP                                |
| Check Seat Availability | Get seat availability of KRISHNA EXP                           |
| Check Live Train Status | Get train live status on date: 2025-07-29, train number: 17230 |

---

### 🚆 Sample Output Summaries

#### 📅 **Schedule: HYD → TPTY (2025-07-31)**

| Train No. | Train Name         | Departs   | Arrives    | Duration | Classes        | Days   |
| --------- | ------------------ | --------- | ---------- | -------- | -------------- | ------ |
| 20701     | TPTY VANDEBHARAT   | 06:10 SC  | 14:35 TPTY | 8h 25m   | EC, CC         | SMWTFS |
| 17230     | SABARI EXPRESS     | 12:20 SC  | 00:00 TPTY | 11h 40m  | 1A, 2A, 3A, SL | Daily  |
| 17406     | KRISHNA EXPRESS    | 06:00 CHZ | 21:40 TPTY | 15h 40m  | 3A, SL, 2S     | Daily  |
| 12797     | VENKATADRI EXPRESS | 20:05 KCG | 06:55 TPTY | 10h 50m  | 1A, 2A, 3A, SL | Daily  |

> **Station Codes**: HYB (Hyderabad), TPTY (Tirupati)

---

### 🔍 Train Info: **KRISHNA EXPRESS (17406)**

* **Route**: ADILABAD → TIRUPATI
* **Distance**: 1227 km
* **Duration**: 24h 35m
* **Key Stops**: Secunderabad, Vijayawada, Gudur, Renigunta
* **Classes**: 3A, CC, SL, 2S, GN
* **Pantry**: No

---

### 🪑 Seat Availability for KRISHNA EXPRESS

| Date       | 3A    | SL   | 2S        |
| ---------- | ----- | ---- | --------- |
| 2025-07-31 | RAC14 | WL33 | WL9       |
| 2025-08-11 | RAC17 | WL12 | AVAILABLE |

**Tip**: Book 3A on July 31 for RAC14, or 2S on August 11 for a confirmed seat.

---

### 📶 Live Train Status: **SABARI EXPRESS (17230)**

#### 📍 On July 29, 2025:

* **Departure**: On-time from Secunderabad
* **Delays**: Up to 38 min at Erode, 28–34 min in Kerala section
* **Arrival**: 8 min **early** at Trivandrum

| Station        | Scheduled | Actual | Status    |
| -------------- | --------- | ------ | --------- |
| Secunderabad   | 12:20     | 12:20  | ✅ On-time |
| Ongole         | 19:24     | 19:51  | ❌ +27 min |
| Ernakulam Town | 11:55     | 12:26  | ❌ +31 min |
| Trivandrum     | 18:05     | 17:57  | ✅ -8 min  |

---

### 📄 License

MIT License

Copyright (c) 2025 lpkumarreddy

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


---
