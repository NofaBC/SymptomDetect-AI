SymptomDetect AI™ — Version 1 Interactive Prototype
A standalone, hospital-blue HTML demo for NOFA AI Factory. Open index.html in a modern browser or deploy it as a static site on Vercel.
Included
- Light hospital-blue dashboard, responsive layout
- English / Spanish / Farsi navigation and core intake translations
- Typed symptom intake and browser-dependent speech recognition
- Optional camera preview, local snapshot capture, and permission controls
- Local image/PDF file preview, manual test-result entry
- Clearly labeled non-live research/case integration blueprint
- Limited keyword-based safety warning demo (not medical triage)
- Downloadable patient-entered visit summary (.txt)
- V1 / V2 JudyDoc™ / V3 PatientRecall AI™ roadmap
Important limitations
- No language model, clinical database, backend, OCR, visual diagnostic model, or research API is connected.
- Uploaded medical documents are not automatically read; images, laboratory results, or patient appearance are not medically interpreted.
- Camera and speech features require a supported browser and explicit user permission. Camera access normally requires HTTPS or localhost. Browser speech recognition may use a cloud service provided by the browser vendor; do not use real patient information for testing.
- The red-flag warning uses only a handful of text patterns. It can falsely flag negated symptoms, miss emergencies, and cannot confirm that any complaint is safe. It must not be relied upon to decide care urgency.
- Do not use this prototype for real clinical decisions or with identifiable patient data. Clinician-led validation, regulatory analysis, security controls, and consent flows are required before clinical use.
- User-entered information is held in page memory only. Downloaded summary files are saved locally at the user's direction. No backend or data persistence is implemented.
Deploy to Vercel
1. Create a repository containing index.html at its root.
2. Import it as a static website into Vercel. No build command or environment variables required.
3. Test voice/camera on a supported browser using HTTPS.
© 2026 NOFA Business Consulting LLC. Conceptual demonstration only.
Mobile medical-document scanning (updated)
In Records & Tests, choose Scan document with phone. On compatible mobile browsers the file input requests the rear camera; other browsers may offer photo selection. The photo previews locally in the same Medical Records area. Use live camera links to the separate consent-based live preview. No OCR, diagnostic interpretation, server upload, or cross-device handoff is implemented. To use a phone, open the deployed HTTPS site on that phone.
Patient information update
A Patient Information navigation step now includes name, DOB, optional demographic/contact details, clinical history, medications and allergies, physician and emergency contact. Entries remain in memory only during the open browser page; no backend or secure medical record exists. The exported text summary includes patient profile fields. Demonstration patient data is synthetic.
