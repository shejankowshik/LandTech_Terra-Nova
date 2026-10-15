# e-Mutation Sahayak (ই-নামজারি সহায়ক)

A small, bilingual (Bangla / English) browser prototype that helps people prepare for a Bangladesh e-Mutation (namjari / kharij) application. It demonstrates a plain-language land-paper guide, transfer-specific document checklist, application steps, sample outcomes, and simple next-step guidance.

## Run it

No installation, server, or build step is needed. Open `index.html` in a current desktop or mobile browser. The prototype uses plain HTML, CSS, and JavaScript, with no runtime packages or external services.

## Try the demo

- Use the language button in the top right to switch between Bangla and English.
- Choose among five fictional cases: a purchase sample marked approved, an inheritance application missing a certificate, a rejection based on the anonymized order pattern shared for this task, a plot-number mismatch, or a case needing specific office review.
- Open **Land papers** to see a glossary, and **Document checklist** to tick the case-specific papers. Checklist changes update the progress indicator.
- Open **Ownership path** to review the selected sample's recorded owner → seller / predecessor → applicant chain. Compare the mouza and plot across the khatian and transfer paper, compare the applicant name with the name written on that paper, and check the recorded area → seller / predecessor share → claimed area. Confirm the document links; the checker flags missing values and possible differences. It is a consistency aid, not a title check.
- Open **Application steps** and **Outcome & next steps** for the process and plain-language sample guidance.
- In **Outcome & next steps**, paste the reason section of an order or load the anonymized sample. A local keyword matcher links familiar Bangla / English phrases to a plain-language meaning and practical next steps. Unrecognized text gets a safe “ask the land office” message.

The preset names, locations, plot numbers, documents, and decisions are invented for demonstration. The hearing example removes all personal details and models the shared order's short labels (“absence” and “incomplete application”) alongside its fuller note that the applicant attended but did not present documentary ownership proof. It explicitly cautions users to read which party and paper the real order identifies. There is no file upload, server-side personal-data collection, account, database, or real application submission. The ownership tool asks users to use sample labels / pseudonyms instead of real names or document numbers. A completed checklist does not determine whether an application will be approved.

The outcome view explains common possible issues in plain language: missing papers, hearing / attendance, gaps in the ownership chain, plot / area / share mismatches, unclear heir shares, court restrictions, and government interests in land. It also notes that a name-spelling difference by itself should not automatically trigger rejection where the NID number matches. For a missing paper, Ministry guidance says the first order should name the exact gap and generally allow 7 working days or a reasonable time; the deadline in the citizen's own notice controls.

## Data and references

The prototype's sample cases are synthetic. The ownership checker does not read uploaded documents or verify legal title; its result is based on the details and confirmation boxes entered by the user. The order explainer uses a small, curated bilingual phrase list in JavaScript; it does not use OCR, an AI service, or a backend. Both tools run in the browser and do not upload or save the entered details. Do not enter real NID numbers or sensitive document identifiers.

The general descriptions and process notes were prepared from publicly available Bangladesh Ministry of Land / DLRS material:

- [Ministry of Land — What is a khatian?](https://minland.gov.bd/pages/static-pages/694032dc35ce18e1c056393d)
- [Ministry of Land — E-Mutation user guide](https://mutation.land.gov.bd/nirdeshika)
- [Ministry of Land — Mutation process steps](https://mutation.land.gov.bd/namjari-steps)
- [Ministry of Land — E-Mutation decisions and rejection reasons (circular compilation)](https://bhumipedia.land.gov.bd/uploads/PDF/Act/All_circular_-14-26_kxKEoQD.pdf)
- [DLRS — Mouza map portal](https://map.settlement.gov.bd/)

The Ministry guide currently describes a ৳70 application and notice fee and a ৳1,100 DCR fee after approval. Fees and procedures may change; the prototype directs users to confirm current instructions on the official portal before paying.

## Technology and AI tools

- **Technology:** HTML, CSS, and vanilla JavaScript. No framework, OCR, backend, or external runtime package is used for this interactive, local-only demonstration.
- **AI tool:** OpenAI Codex assisted with implementation, bilingual draft copy, and preparation of the project documentation. No AI model or API runs inside the prototype.
