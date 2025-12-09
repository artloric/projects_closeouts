# ACEN–UFS merSETA Risk Register

This repository contains a professional, hybrid **PMI / Agile** risk register for the:

> **Circular Economy Training for the South African Manufacturing Sector**  
> ACEN – University of the Free State (UFS) – merSETA project

The register has been reconstructed as if it were prepared **at project inception**, using the final project documentation as reference. It is designed for use in a **Project Management portfolio**, GitHub profile, or as supporting evidence for **PMI / Agile** capability.

## Repository Contents

- `README.md` – this overview and usage guide.
- `risk-register.md` – human-readable Markdown risk register, suitable for GitHub and documentation.
- `risk-register.csv` – CSV version for quick imports.
- `risk-register.xlsx` – Excel workbook with:
  - **Risk Register** sheet (all risks, attributes, and owners)
  - **Risk Summary** sheet (Risk Type × Severity pivot)
  - **Heatmap** sheet (5×5 risk matrix with conditional formatting)
- `heatmap.png` – visual **5×5 risk matrix** (Likelihood × Impact) using a classic green–yellow–red gradient.
- `mermaid-heatmap.md` – Mermaid.js snippet for embedding a heatmap directly in Markdown (for GitHub, MkDocs, or similar).

## Methodology

The risk register is structured according to a **hybrid project management approach**:

- **PMI / PMBOK-style** risk identification, qualitative analysis, and documentation.
- **Agile practices** for iterative validation, sprint-level risk monitoring, and lightweight governance.
- Alignment to the project’s actual **deliverables and workstreams**, including:
  - C3.x – Desktop Research & Training Needs
  - C4.x – Webinars & Awareness
  - C5.x / C6 – Training Frameworks & Materials
  - C8–C10 – Case Studies
  - C11–C15 – Training Delivery
  - C16 – Project Close-Out

Each risk is tied to specific deliverables and grouped logically by workstream, making it easy to see how risk exposure shifts across the life cycle.

## Risk Scoring

- **Probability**: Low / Medium / High (qualitative)
- **Impact**: Low / Medium / High (qualitative)
- **Score**: Numeric (1–25), based on a simple Likelihood × Impact scale
- **Severity bands**:
  - 1–5   → Low
  - 6–10  → Medium
  - 11–15 → High
  - 16–25 → Critical

These bands are reflected in the Excel workbook and the 5×5 heatmap.

## How to Use This in a Portfolio

You can use this repository to demonstrate that you:

- Design **deliverable-based risk structures** aligned with a Work Breakdown Structure (WBS) or feature map.
- Apply **qualitative risk analysis** and communicate using both tabular and visual tools.
- Understand **complex, policy-heavy research and training projects**, with multiple stakeholders (ACEN, UFS, merSETA, government, and industry).
- Work comfortably in both **traditional** and **Agile** environments.

Suggested talking points in an interview:

- How you would keep this register **alive** in sprints (e.g., risk review during sprint planning and review).
- How you would prioritise and escalate **critical** risks (Score ≥ 16).
- How this type of register supports **benefits realisation** and **lessons learned** at close-out.

## Getting Started

1. **Download the Excel file** and open `risk-register.xlsx` in Excel or LibreOffice.
2. Review the **Risk Register** sheet and filter by:
   - Workstream / Deliverable
   - Risk Type
   - Severity
3. View the **Risk Summary** sheet to see how risk is distributed across types.
4. Use the **Heatmap** sheet and `heatmap.png` when presenting to stakeholders.

## Embedding the Mermaid Heatmap

See `mermaid-heatmap.md` for a Mermaid.js heatmap snippet you can paste directly into GitHub or documentation generators that support Mermaid.

---

If you would like a variant of this risk register (e.g., **different scoring model**, **Scrum-only framing**, or a **Jira import template**), the structure allows easy extension.
