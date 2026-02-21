# 🛡️ CMMC Level 1 Self-Assessment Tool

![CMMC Level 1](https://img.shields.io/badge/CMMC-Level%201-0066ff?style=for-the-badge&logo=shield&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-Single%20File-e34f26?style=for-the-badge&logo=html5&logoColor=white)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-00e676?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

A fully client-side, single-file CMMC Level 1 self-assessment tool built for GRC engineers, compliance analysts, and cybersecurity professionals preparing for DoD contractor compliance. No backend, no install, no data ever leaves your browser.

---

## 📸 Preview

> Open `cmmc-l1-assessment.html` directly in any modern browser — no server required.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎯 **17 Practices** | All CMMC Level 1 practices across all 6 domains |
| 📊 **Live Dashboard** | Real-time compliance score with animated ring chart and per-domain progress bars |
| 📋 **Full Guidance Panels** | Click any control ID to expand objective, key activities, assessment methods, and references |
| ✅ **Toggle Responses** | Mark each practice Yes / No / N/A — click again to deselect |
| 📝 **Evidence & Notes** | Expandable notes panel with large text area per control |
| 📎 **File Attachments** | Attach PDFs, Word docs, Excel, CSVs, and images as evidence |
| 💾 **Auto-Save** | Progress saved automatically to browser localStorage |
| 📤 **Export Report** | Generate and download a formatted `.txt` assessment report |
| 🔍 **Filter View** | Filter by All / Unanswered / Non-Compliant |
| ⚖️ **Smart Scoring** | N/A practices excluded from compliance denominator |

---

## 🗂️ CMMC Level 1 Domains Covered

| Domain | Code | Practices |
|---|---|---|
| Access Control | AC | 4 |
| Identification & Authentication | IA | 2 |
| Media Protection | MP | 1 |
| Physical Protection | PE | 4 |
| System & Communications Protection | SC | 2 |
| System & Information Integrity | SI | 4 |
| **Total** | | **17** |

---

## 🚀 Getting Started

### Option 1 — Direct Download
1. Download `cmmc-l1-assessment.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Start assessing — your progress saves automatically

### Option 2 — Clone the Repo
```bash
git clone https://github.com/Orlando-GRCengineer/cmmc-l1-assessment.git
cd cmmc-l1-assessment
open cmmc-l1-assessment.html
```

No `npm install`. No build step. No server. Just open and go.

---

## 🧭 How to Use

### 1. Assess Each Practice
For each of the 17 practices, select your compliance status:
- **✓ Yes** — Control is implemented (green)
- **✕ No** — Control is not implemented (red) — creates a gap
- **— N/A** — Not applicable to your environment (yellow)

Click the same button again to deselect.

### 2. View Guidance
Click **▶ GUIDANCE** on any practice to expand full detail including:
- Plain-English objective
- Key implementation activities
- Assessment methods used by assessors
- Regulatory references (NIST SP 800-171, FAR, NIST 800-53)

### 3. Add Evidence
Click **📋 Evidence / Notes** to expand the evidence panel where you can:
- Write detailed notes about your implementation
- Attach supporting files (PDF, DOCX, XLSX, CSV, TXT)
- Attach screenshots and images as evidence
- See a live character and file count badge

### 4. Track Your Score
The dashboard updates live as you answer:
- **Compliance ring** shows your overall % score
- **Domain bars** show progress per domain
- **Status badge** shows gap count or full compliance

### 5. Export Your Report
Click **Export Report** in the header to generate a formatted summary including all responses, scores per domain, and your evidence notes. Download as `.txt` or copy to clipboard.

---

## 📐 Scoring Methodology

Compliance percentage is calculated as:

```
Score = (Yes Count) / (Total Practices - N/A Practices) × 100
```

Practices marked **N/A** are excluded from the denominator, consistent with how SPRS self-assessment scoring is typically handled for Level 1.

---

## 📁 Project Structure

```
cmmc-l1-assessment/
├── cmmc-l1-assessment.html   # Complete tool — single self-contained file
└── README.md                 # This file
```

---

## 🔒 Privacy & Data Handling

- **All data stays local** — nothing is ever transmitted to any server
- **localStorage only** — text responses saved to your browser's local storage
- **File attachments** — stored in memory only for the current session (not persisted)
- **No analytics, no tracking, no external calls** (except Google Fonts for typography)

---

## ⚖️ Regulatory References

| Reference | Description |
|---|---|
| [CMMC Program](https://dodcio.defense.gov/CMMC/) | DoD Cybersecurity Maturity Model Certification |
| [NIST SP 800-171 Rev 2](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) | Protecting CUI in Nonfederal Systems |
| [FAR 52.204-21](https://www.acquisition.gov/far/52.204-21) | Basic Safeguarding of Covered Contractor Information Systems |
| [32 CFR Part 170](https://www.ecfr.gov/current/title-32/part-170) | CMMC Program Rule |
| [SPRS Portal](https://www.sprs.csd.disa.mil/) | Supplier Performance Risk System |

---

## ⚠️ Disclaimer

This tool is provided for **self-assessment and preparation purposes only**. It does not constitute an official CMMC assessment and confers no certification status.

- CMMC Level 1 certification requires an **annual self-assessment** affirmed by a Senior Company Official and submitted to **SPRS**
- An official **C3PAO assessment is not required** for Level 1, but the self-assessment must meet all DoD requirements
- This tool is not affiliated with, endorsed by, or approved by the DoD, CMMC-AB, or any official certifying body

---

## 🛠️ Built With

- Vanilla HTML, CSS, JavaScript — zero frameworks, zero dependencies
- [IBM Plex Mono & IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Mono) — Google Fonts
- CSS Grid animations for smooth accordion panels
- localStorage API for client-side persistence

---

## 🤝 Contributing

Contributions are welcome! Some ideas for enhancements:

- [ ] POA&M (Plan of Action & Milestones) tracker
- [ ] Remediation guidance and recommended tools per practice
- [ ] Export to Excel / PDF
- [ ] CMMC Level 2 practices (110 practices from NIST SP 800-171)
- [ ] Multi-assessment comparison view
- [ ] Dark/light theme toggle

To contribute:
```bash
git fork https://github.com/Orlando-GRCengineer/cmmc-l1-assessment.git
git checkout -b feature/your-feature-name
# Make your changes to cmmc-l1-assessment.html
git commit -m "feat: add your feature description"
git push origin feature/your-feature-name
# Open a Pull Request
```

---

## 📄 License

MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

## 👤 Author

Built for the GRC and cybersecurity community by practitioners who needed a fast, clean, no-nonsense CMMC Level 1 readiness check.

> ⭐ If this tool helped you, please star the repo!

---

*Version 1.0.0 · CMMC Level 1 · 17 Practices · 6 Domains*
