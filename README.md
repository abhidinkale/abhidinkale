# Abhi Dinkale

Building **Proton** — a clinical copilot where AI proposes and the physician attests.

[Validation Suite](https://github.com/abhidinkale/proton/blob/main/docs/VALIDATION.md) • [Known Issues & Tech Debt](https://github.com/abhidinkale/proton/blob/main/docs/KNOWN_ISSUES.md) • [Interactive Preview](https://github.com/abhidinkale/proton-trailer)

---

### What Works Today (Proton)
Proton is an AI-assisted clinical workstation built around physician attestation and deterministic safety verification:
- **Safety-Gated Clinical Notes**: Real-time ambient dialogue capture and structured SOAP drafting. AI proposals carry explicit provenance badges until reviewed, edited, or attested by the physician.
- **Deterministic Clinical Verification**: Rule-based safety engine that strictly blocks invalid prescriptions (missing dosage, frequency, duration) and flags cross-reactive allergy conflicts prior to submission.
- **FHIR R4 Persistence**: Encounter notes, active conditions, and care plans are mapped directly into standard Medplum / FHIR R4 resources.
- **Offline-First Android Patient App**: Mobile companion with local SQLite/Room storage, OS alarm-driven background sync, and clinic link-code pairing.

> **Synthetic Data Notice**: Proton is tested and validated exclusively against synthetic patient cohorts. Production deployment with Protected Health Information (PHI) requires enterprise BAAs, tenant isolation, and production KMS encryption.

### Roadmap
- **On-Device Acoustic Transcription**: Quantized local models (moving beyond cloud AI gateways).
- **Hardware-Backed Encryption**: SQLCipher local storage encryption for disconnected clinic devices.
- **Degraded Local Network Mesh**: Resilient offline sync for rural clinics with intermittent connectivity.

---

### Stack
- **Mobile**: Kotlin, Jetpack Compose, Room, WorkManager, Coroutines & Flow
- **Web**: TypeScript, React, Tailwind CSS, Vite
- **Backend & Data**: Node.js, Express, PostgreSQL, Medplum / FHIR R4
- **Verification**: Deterministic test suites (185+ unit tests, automated CI validation)

---

### Public Repositories
- [**proton**](https://github.com/abhidinkale/proton) — Clinical copilot where AI proposes and the physician attests.
- [**proton-trailer**](https://github.com/abhidinkale/proton-trailer) — Interactive preview and walkthrough of the clinical workstation.
- [**developer-journal**](https://github.com/abhidinkale/developer-journal) — Architecture decision records (ADRs), daily engineering logs, and reflections.
- [**daily-selfie-app**](https://github.com/abhidinkale/daily-selfie-app) — Timelapse camera with fluid mass-spring-damper physics in React Native.
- [**project-arc**](https://github.com/abhidinkale/project-arc) — Clinical agent workflow prototype for note drafting, triage, and task execution.

---

### Pilot Plan
Running a focused **30-day pilot across 1–3 community clinics** using synthetic test cohorts to validate physician attestation speed, workflow integration, and deterministic safety guardrails.

---

**Contact**: [abhidinkale@gmail.com](mailto:abhidinkale@gmail.com) • [X / Twitter (@mysticgecko)](https://x.com/mysticgecko)
