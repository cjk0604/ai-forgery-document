# Multimodal Gemini Document Forgery Detection Practice

This repository contains Jupyter Notebook practice guides for building a high-precision document forgery and alteration detection pipeline. The pipeline uses the latest Google GenAI SDK and Gemini models (such as `gemini-3.5-flash` or `gemini-3.5-pro`) to scan documents (receipts, invoices, transaction screenshots) for signs of digital tampering.

## 📂 Project Structure

- **[gemini_document_forgery_detection_practice.ipynb](file:///Users/changjoon/Documents/04_Coupang/07_ai_forgery_2/gemini_document_forgery_detection_practice.ipynb)**: Korean version of the hands-on practice notebook.
- **[gemini_document_forgery_detection_practice_en.ipynb](file:///Users/changjoon/Documents/04_Coupang/07_ai_forgery_2/gemini_document_forgery_detection_practice_en.ipynb)**: English version of the hands-on practice notebook.

## 🚀 Getting Started

### Prerequisites

You need a Google Gemini API Key (AI Studio) or a Google Cloud Project with Vertex AI enabled (IAM auth).
Ensure you have the required Python libraries installed:
```bash
pip install google-genai pandas pillow matplotlib openpyxl
```

### Steps to Run

1. **Open the Notebook**: Open either the Korean or English version of the notebook in Google Colab or your local Jupyter environment.
2. **Client Initialization (Step 2)**:
   - Configure either the `API_KEY` (for Google AI Studio) or `PROJECT_ID` / `LOCATION` (for Vertex AI IAM authentication).
3. **Load and Visualize Images (Step 3)**:
   - **Colab**: Upload files interactively using the upload prompt.
   - **Local Workspace**: Place your sample receipt/invoice images under a folder named `허위서류 공유` (Shared Forged Documents) or directly in the current directory.
4. **Forensic Analysis Pipeline (Step 4 & 5)**:
   - Define system instructions and the JSON output schema constraints.
   - Run the evaluation loop to batch process images and view structured forensic reports.
