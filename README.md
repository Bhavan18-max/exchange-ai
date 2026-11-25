# Xchange AI — FOREXWISE

> **AI-Powered Currency Exchange Comparison Platform**  
> Academic FinTech prototype by Team City Spark

---

## Project Overview

**Xchange AI** helps users compare foreign-exchange quotations in a consistent, transparent format. It brings together real-time rate lookups, fee calculations, provider comparisons, regulatory-document retrieval (RAG), risk indicators, and human review — all in one browser-based app.

> ⚠️ **Educational demo only.** Not an RBI-authorised money changer. Rates, transactions and fees shown are fictional/demo data.

---

## Features

| Feature | Description |
|---|---|
| 🧮 **Exchange Calculator** | Buy or sell foreign currency with fees & GST itemised |
| 🤖 **AI Provider Compare** | Multi-agent AI ranks 7 fictional providers on cost, fees, trust and risk |
| 📊 **Currency Rates vs ₹** | All 10 major currencies vs Indian Rupee |
| 📈 **Trade Graph** | Simulated live currency price movement chart |
| 📋 **Transaction History** | Filter, search, and export (CSV) demo transactions |
| 📜 **RBI Rules & KYC** | Key regulatory info: FEMA, KYC, AML & CFT |
| 🧠 **RAG Agent** | Retrieves relevant passages from built-in RBI/FEMA/KYC knowledge base |
| 🔐 **Auth (Demo)** | Demo login/register with OTP (shown on screen, no real SMS) |
| 🌐 **Multi-language** | English, Hindi, Telugu, Tamil, Kannada, Malayalam, Bengali |
| 🌙 **Dark mode** | Auto-detects system preference |

---

## Multi-Agent Architecture

```
Supervisor Agent
├── Rate Agent          → Checks reference rate and source
├── Comparison Agent    → Ranks providers by effective total cost
├── Risk Agent          → Checks verification, rate anomalies, risk score
└── Recommendation Agent→ Selects the best eligible verified provider
```

The **Supervisor** coordinates all agents, validates the result, and approves only a recommendation that passes every check.

---

## Project Structure

```
exchange ai/
├── index.html          # Main SPA entry point
├── assets/
│   ├── style.css       # All styles (dark mode, responsive, components)
│   └── app.js          # All logic (agents, chart, auth, history, RAG)
├── README.md           # This file
└── site_raw.html       # Original source (reference)
```

---

## Running the Project

**Option 1 — Open directly:**
```
Double-click index.html
```

**Option 2 — Local dev server (recommended for fetch-based features):**
```bash
# Using Python
python -m http.server 3000

# Using Node.js
npx serve .

# Then open http://localhost:3000
```

---

## Demo Credentials

| Role | Mobile | Password |
|---|---|---|
| Customer | `9876543210` | `demo123` |
| Admin | `9999999999` | `admin123` |

OTP is displayed on-screen — no real SMS is sent.

---

## Supported Currencies

| Code | Currency |
|---|---|
| USD | 🇺🇸 US Dollar |
| EUR | 🇪🇺 Euro |
| GBP | 🇬🇧 British Pound |
| AED | 🇦🇪 UAE Dirham |
| SGD | 🇸🇬 Singapore Dollar |
| JPY | 🇯🇵 Japanese Yen |
| AUD | 🇦🇺 Australian Dollar |
| CAD | 🇨🇦 Canadian Dollar |
| CHF | 🇨🇭 Swiss Franc |
| SAR | 🇸🇦 Saudi Riyal |

---

## Official Reference Data Sources

The platform links to official rate sources for the Rate Agent:

- **RBI Reference Rate Archive** — Historical Indian reference rates
- **FBIL** — Official benchmark administrator for major-currency INR rates (from 10 Jul 2018)
- **Frankfurter API** — Live & historical reference rates (fetched directly)
- **ECB Reference Rates** — EUR-based daily reference rates
- **RBI DBIE** — Indian economic and financial time series

---

## SDG Alignment

| SDG | Goal | Alignment |
|---|---|---|
| SDG 8 | Decent Work & Economic Growth | Primary fit — informed access to FX info |
| SDG 9 | Industry, Innovation & Infrastructure | Supporting fit — AI agents, RAG, FinTech |
| SDG 16 | Peace, Justice & Strong Institutions | Supporting fit — transparency, regulatory grounding |

---

## Team

**Team Name:** City Spark  
**Members:** M. Mahathi Tanmayi · T. Kartikeya · Ch. Anvitha · Bhavan K · G. Krishna Sai

---

## Disclaimer

This is an educational demo prototype. Not legal advice. Not an RBI-authorised money changer. All rates, provider data, and transactions are fictional. Always verify with authorised entities at [rbi.org.in](https://rbi.org.in).
