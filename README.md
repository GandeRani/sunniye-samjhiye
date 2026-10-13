\# Sunniye, Samjhiye — AI-Powered Patient Intake Storyteller



\*\*Listen to Every Patient. Understand Every Story.\*\*



Sunniye, Samjhiye is an AI-powered prototype designed to help organize patient narratives and medical documents into structured clinical note drafts. It explores how speech AI, OCR, and large language models can support patient intake and reduce manual documentation effort.



\## Problem



During outpatient department (OPD) intake, patient narratives and existing medical documents can be difficult to organize quickly. Language differences, handwritten prescriptions, and unstructured information may make clinical documentation more time-consuming.



\## Solution



The prototype uses Sarvam AI to process audio and medical documents, then generates structured summaries for clinician review.



\## Features



\- \*\*Speech transcription:\*\* Converts supported-language patient audio into text using Sarvam AI.

\- \*\*Medical document OCR:\*\* Extracts text from uploaded documents using document digitisation.

\- \*\*AI-generated summaries:\*\* Organizes extracted information into a structured clinical note draft.

\- \*\*Review-focused output:\*\* Flags ambiguous or uncertain information for human verification.

\- \*\*Human-in-the-loop approach:\*\* Treats generated notes as drafts, not as a replacement for professional clinical judgment.



\## Tech Stack



\- Python

\- FastAPI

\- Sarvam AI APIs

\- HTML, CSS, and JavaScript

\- Uvicorn



\## Project Structure



```text

sunniye-samjhiye/

├── main.py

├── requirements.txt

├── .gitignore

├── README.md

└── static/

&#x20;   └── index.html

```



\## Getting Started



\### 1. Clone the repository



```bash

git clone https://github.com/GandeRani/sunniye-samjhiye.git

cd sunniye-samjhiye

```



\### 2. Create and activate a virtual environment



On Windows PowerShell:



```powershell

python -m venv .venv

.\\.venv\\Scripts\\Activate.ps1

```



\### 3. Install dependencies



```powershell

pip install -r requirements.txt

```



\### 4. Configure the API key



Create a `.env` file in the project root and add your own Sarvam API key:



```text

SARVAM\_API\_KEY=your\_sarvam\_api\_key\_here

```



Never commit your real API key or `.env` file to GitHub.



\### 5. Run the application



```powershell

python -m uvicorn main:app --reload

```



Open `http://127.0.0.1:8000` in your browser.



API documentation is available at `http://127.0.0.1:8000/docs`.



\## Responsible Use



This project is a prototype for exploring AI-assisted clinical documentation. AI-generated text can contain errors and must be reviewed by a qualified healthcare professional. Do not use it as a substitute for diagnosis, treatment decisions, or professional medical judgment. Use synthetic or properly de-identified data for testing.



\## Future Improvements



\- Better source-level traceability for extracted clinical facts.

\- Clear separation of source-supported information and uncertain interpretations.

\- Improved multilingual patient intake workflows.

\- Clinician review and sign-off features.



\## Author



\*\*Gande Rani\*\*



GitHub: \[@GandeRani](https://github.com/GandeRani)

