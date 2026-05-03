# 🤖 Palyam IQ
### AI-Assisted Enterprise Integration Diagnostics Platform (Prototype)

> **Disclaimer:** This is a simplified representation of the system. Core algorithms,
> AI models, and internal logic are intentionally abstracted and not included.

---

## The Problem

Debugging failures in Oracle Integration Cloud (OIC2 / OIC3) environments is
time-consuming and complex. Integration engineers often spend hours manually
searching documentation, forums, and logs to identify root causes — slowing
down incident response and increasing operational costs.

---

## What It Does

Palyam IQ is an AI-assisted diagnostics system that accepts integration errors
or log inputs from OIC environments and returns structured root cause suggestions
and recommended fixes — in seconds, not hours.

Designed to augment integration engineers by accelerating root cause identification, reducing mean time to resolution (MTTR), and improving system reliability.

> **Prototype demonstrates significant reduction in debugging time: hours → seconds.**

---

## High-Level Architecture

```
[ OIC Logs / Error Inputs ]
          ↓
   [ Data Ingestion Layer ]
   OIC2 / OIC3 error capture
          ↓
    [ Preprocessing Layer ]
    Normalisation · Context tagging
          ↓
    [ Analysis Layer ]
    Error analysis (abstracted)
          ↓
    [ Reasoning Layer ]
   AI-assisted reasoning (abstracted)
          ↓
  [ Structured Output ]
  Root Cause · Affected Components · Suggested Fix
```

---

## Key Capabilities

| Capability | Description |
|---|---|
| OIC2 + OIC3 Support | Works across both integration platform generations |
| Faster Debugging | Reduces manual investigation from hours to seconds |
| Root Cause Suggestions | Surfaces likely causes based on error context |
| Affected Component Mapping | Identifies impacted APIs, adapters, and systems |
| Structured Output | Consistent, readable response format for every query |
| Reduced Manual Effort | Eliminates repeated searching of forums and documentation |

---

## Sample Interaction

**Input:** `Authentication token expired during enterprise API request`

**Output:**
- **Error Summary:** Token expiry during outbound REST API call
- **Suggested Cause:** OAuth access token exceeded validity period
- **Affected Components:** ERP Cloud REST API · OIC3 Platform
- **Recommended Fix:** Implement token refresh logic and validate expiry
  before API invocation
- **Related Patterns:** SSL handshake failures · Authentication config errors

---

## Tech Stack (High Level)

| Layer | Technology |
|---|---|
| Backend | Python · FastAPI |
| Frontend | React · Vite · Tailwind CSS |
| Database | Data storage (abstracted) |
| AI Layer | AI-assisted analysis (abstracted) |
| Deployment | Local prototype |

---

## Status

🧪 Prototype — built to validate the core diagnostic concept and demonstrate a working system with structured diagnostic outputs and a repeatable analysis flow.

Covers a wide range of common integration error scenarios across OIC2 and OIC3
error categories including REST, SOAP, FTP, Scheduler, SSL, B2B, and DB adapters.

---

## About

Built by **Palyam IQ** 

📧 support@palyamiq.com
