# Baiduri Capital – Complex ETF Identifier


**Here is the link to the website:**  
[Open Complex Securities Identifier](https://hafizzankadir.github.io/ComplexSecurities_Identifier/)

Testing API Key = AQ.Ab8RN6IZxRNIgi-Ni56S6EgITobu_C5K8a2tLlocy3uu0s0TAQ

A client-side AI-powered web application for identifying and classifying ETFs based on their exposure to complex securities and derivative strategies. The system retrieves official factsheets, determines country of domicile, and provides confidence-scored compliance insights.

---

## Overview

The Complex ETF Identifier automates ETF due diligence by:

- Detecting complex financial instruments:
  - Derivatives (options, swaps, futures)
  - Leveraged or inverse strategies
  - Synthetic replication structures  
- Identifying the ETF's country of domicile
- Retrieving official factsheets or fallback product pages
- Generating compliance-grade commentary
- Assigning a confidence score based on source reliability

All analysis is powered by Google Gemini AI and runs entirely in the browser.

---

## Key Features

### ETF Classification
- Complex
- Non-Complex
- Pending / Error

### Country Identification
- Full country name
- ISO country code

### Factsheet Retrieval
- Official PDF (preferred)
- Product page fallback

### Confidence Scoring

| Score | Description |
|------|------------|
| 90–100 | Verified factsheet PDF |
| 70–85 | Strong product page |
| 50–65 | Partial / inferred |
| 30–45 | Weak verification |
| 10–25 | No reliable source |

---

## Tech Stack

| Component | Technology |
|----------|-----------|
| UI | Tailwind CSS |
| AI | Google Gemini API |
| Data | XLSX.js |
| Runtime | HTML + JavaScript |

---

## Setup Instructions

### Step 1 – Open Application

open index.html

## Step 2 – Configure API Key

- Click **Analysis Settings**
- Enter your **Gemini API Key**
- Get from: https://aistudio.google.com/

**Select model:**
- `gemini-2.5-flash` (recommended)
- `gemini-2.5-pro`

---

## How to Use

### Step 1 – Load Data

**Option A: Upload Spreadsheet**
- Upload `.xlsx`, `.csv`, or `.xls`
- Select ticker column

**Option B: Manual Entry**
- Enter tickers line-by-line
- Click **Load Manual List**

---

### Step 2 – Start Analysis

Click **"Start Automated Analysis"**

**System will:**
- Retrieve factsheet or product page
- Identify country
- Classify ETF
- Generate commentary
- Assign confidence score

---

### Step 3 – Monitor Progress

- View progress bar
- Track logs in console
- Use pause/resume controls

---

### Step 4 – Review Results

**Filter using:**
- Classification (Complex / Non-Complex)
- Country
- Confidence threshold

---

### Step 5 – Re-run ETF Analysis

Click **refresh icon** beside ticker

- Re-analyzes selected ETF
- Updates classification and commentary

---

### Step 6 – Export Results

- Export Excel dataset
- Generate PDF report

---

## Prompt Customisation

### How to Modify

- Open **Analysis Settings**
- Edit **Custom Analysis Prompt**
- Click **Apply Configs**

---

### Example Prompt
- Highlight all derivative usage clearly
- Identify counterparty risks for swaps
- Focus on regulatory concerns
- Limit output to 2 concise bullet points

---

### Best Practices

- Keep instructions concise
- Avoid ambiguity
- Base on factsheet evidence only

---

## Cost Estimation

**Estimated API usage:**
- $0.10 per 100 tickers

### Cost Examples

| Tickers | Cost  |
|--------:|------:|
| 100     | $0.10 |
| 500     | $0.50 |
| 1,000   | $1.00 |

## Cost Estimation

**Estimated API usage:**
- $0.15 per 100 tickers

### Cost Examples

| Tickers | Cost  |
|--------:|------:|
| 100     | $0.15 |
| 500     | $0.75 |
| 1,000   | $1.50 |

## Cost Estimation

**Estimated API usage:**
- $0.20 per 100 tickers

### Cost Examples

| Tickers | Cost  |
|--------:|------:|
| 100     | $0.20 |
| 500     | $1.00 |
| 1,000   | $2.00 |
---

## Input Format

### Minimum Example

Ticker
SPY
QQQ
VTI

---

## Output Fields

- Ticker
- Country
- ISO Code
- Factsheet URL
- Classification
- Commentary
- Confidence Score

---

## Use Cases

- Compliance auditing
- ETF classification
- Investment due diligence
- Regulatory reporting

---

## Limitations

- Depends on factsheet availability
- AI interpretation may vary
- Manual review may be required

---

## Security

- API key stored locally
- No backend required
- No stored data
