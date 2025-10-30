# PV Narrative Practice Tool

An interactive, single-page web application for practicing pharmacovigilance (PV) case narratives. The tool presents synthetic unsolicited cases and provides structured guidance and objective feedback to help authors produce clear, compliant, regulator-ready narratives.

## Overview

- **Scope:** Post-marketing unsolicited cases with a mix of AE, SAE, and serious-unexpected (SUSAR-type) scenarios.
- **Structure:** Argus-style data confirmation, free-text narrative drafting, automated checks, and a rubric-based report.
- **Audience:** PV associates, medical writers, QA/medical reviewers, and trainees seeking hands-on practice.

## Key Features

- **10 synthetic cases** (unsolicited), covering diverse scenarios and complexity.
- **Argus-style form** for essential fields (patient, suspect drug, event details, chronology, labs, actions, outcome, dechallenge/rechallenge).
- **Narrative editor** with word-count target and prompts.
- **Automated feedback**:
  - *Must-Fix* (compliance-critical items).
  - *Should-Improve* (quality/clarity suggestions).
- **Scoring rubric (/20)** assessing completeness, chronology, drug details, event course, dechallenge/rechallenge, confounders, investigations (with units/dates), seriousness/expectedness, tone, and internal consistency.
- **Model narrative** (JSON-driven) for comparison.
- **Local autosave** per case; runs entirely client-side.

## Live Demo

- **GitHub Pages:** https://soumyadubey.github.io/pv-narrative-practice/

## Usage

1. Select a case from the dropdown.
2. Review the vignette and confirm key fields.
3. Draft a concise, neutral narrative (target 120–180 words).
4. Submit to view the report, including Must-Fix items, quality suggestions, and score.
5. Compare with the model narrative and iterate as needed.

## Data & Privacy

- All cases are **synthetic** for training purposes.
- No personal health information (PHI) is collected or stored.
- The application runs locally in the browser; no backend services are used.

## Technology

- Single-file **HTML/CSS/JavaScript**.
- Static hosting via **GitHub Pages**.

## Limitations

- The rules engine is heuristic and conservative; it supports training but does not replace human medical review or regulatory judgment.

## License

MIT License. See `LICENSE` for details.
