# IIH Manager — Clinical Decision Support

**A mobile-first point-of-care tool for optometrists and ophthalmologists managing idiopathic intracranial hypertension (IIH)**

> Developed by **Steven C. Quan OD FAAO**  
> Assistant Professor of Ophthalmology & Visual Science  
> University of Chicago Medicine  
> Program Director, Optometry Residencies & Externships

---

## Overview

IIH Manager is a standalone, offline-capable clinical decision support web app designed for use at the point of care. It is intended for both experienced neuro-ophthalmologists and general optometrists or ophthalmologists who encounter IIH less frequently.

The app runs entirely in the browser — no installation, no login, no data transmission. Patient tracking data is stored locally on the user's device only.

---

## Features

### 🔬 Diagnose
- LP opening pressure visual gauge with obesity-adjusted threshold (≥250 / ≥280 mm H₂O)
- Built-in cm H₂O → mm H₂O unit converter
- BMI calculator that auto-populates the pressure threshold
- Interactive Modified Dandy Criteria checklist (Friedman 2013) with automatic IIH / IIHWOP / Probable IIH classification
- OCT RNFL corroborating evidence module with context-aware interpretation (new diagnosis, follow-up, IIHWOP evaluation)

### 🚦 Triage
- **Papilledema Spotter** — first-encounter urgency routing for less-experienced clinicians (bilateral vs. unilateral, vision threat, neurological symptoms, prior workup, BP, pediatric flag)
- **Pseudopapilledema Differentiator** — weighted feature scoring to distinguish true disc edema from disc drusen and anatomic variants
- **Secondary Causes Checklist** — 11 clinically framed questions with evidence-stratified interpretation (tetracyclines, retinoids, OSA, thyroid, iron deficiency, CVT, and others)

### 💊 Treat
- Five-node first-line treatment decision tree (vision threat, pregnancy, sulfa allergy, renal function, vision risk stratification)
- IIHTT acetazolamide titration calculator with patient age–corrected MDRD GFR estimation
- Weight management module with GLP-1 and bariatric surgery considerations
- LP timing decision tool (therapeutic, diagnostic, and bridging indications)
- Side effect management for 7 common acetazolamide adverse effects
- RNFL surgical escalation threshold calculator (>5 µm from baseline)
- Surgical escalation deep reference: ONSF, CSF shunting, TVS stenting — with post-operative monitoring schedules and failure mode recognition

### 📈 Track
- Anonymous longitudinal patient tracker (localStorage — no PHI transmitted)
- Fields: weight, VA OD/OS, LP OP, RNFL OD/OS, acetazolamide dose, papilledema grade, GHT, VF mean deviation OD/OS, notes
- Automatic RNFL baseline vs. current delta with >5 µm surgical escalation alert
- Trend charts for LP OP, weight, and RNFL over time
- Patient list view with visit count and last visit date
- CSV export for all visit data

### 📖 Reference
- Frisén Scale grading guide (Grades 0–5) with clinical action at each grade
- IIH monitoring timeline (Baseline → 4–6 weeks → 3 months → 6 months → Annual)
- Referral letter generator with copy and print/share functionality
- Plain-language patient summary generator with customizable return-to-ER warning signs

---

## Clinical Basis

- Friedman DI et al. Revised diagnostic criteria for the pseudotumor cerebri syndrome in adults and children. *Neurology.* 2013;81(13):1159–1165.
- IIHTT Study Group. Effect of Acetazolamide on Visual Function in Patients with Idiopathic Intracranial Hypertension and Mild Visual Loss. *JAMA.* 2014;311(16):1641–1651.
- NORDIC Idiopathic Intracranial Hypertension Study Group guidelines.
- De Lott LB et al. Levonorgestrel intrauterine device use and incident idiopathic intracranial hypertension. *Contraception.* 2023;125:110089.

---

## Data & Privacy

- **No data is transmitted.** All patient tracking data is stored in the user's browser localStorage.
- **No PHI should be entered.** Use anonymous patient identifiers only (e.g., IIH-001).
- The app contains no analytics, tracking, or third-party scripts.

---

## Disclaimer

IIH Manager is a clinical decision support tool intended for use by trained clinicians only. It does not replace clinical judgment, formal ophthalmic examination, or specialist consultation. It has not been validated for autonomous diagnostic use and is not FDA cleared.

---

## Install as a Mobile App

Open the URL in **Safari on iPhone** → tap the Share icon → **Add to Home Screen**. The app launches full-screen and works offline. No App Store required.

---

## Contributing / Feedback

This tool is in active development. Feedback from clinicians — particularly regarding clinical accuracy, workflow fit, and feature gaps — is welcome via GitHub Issues.

---

*IIH Manager is not affiliated with or endorsed by the University of Chicago Medicine, the American Academy of Optometry, or any pharmaceutical company.*
