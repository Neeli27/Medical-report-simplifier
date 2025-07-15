## Medical Report Simplifier — PDF/Image/Text Extraction + LLaMA 3 via Groq
This project simplifies complex medical reports into easy-to-understand language using the LLaMA 3 (70B) model hosted on Groq. It supports input in the form of PDFs, images, or plain text files, making it useful for patients and non-medical users.
## Key Features
Built with LLaMA 3 (70B) via Groq for fast and human-like medical text simplification.
Multi-format input support extract medical content from PDF, image, or text files.
OCR and preprocessing using PyMuPDF and Tesseract for accurate content extraction.
User-friendly output that avoids medical jargon and explains things clearly.
Google Colab friendly no deployment required, easy to run and experiment.
## How It Works
Upload File: Choose between uploading a `.pdf`, `.jpg/.png`, or `.txt` file.
Text Extraction:
   - For PDFs → uses `PyMuPDF`
   - For images → uses `Tesseract OCR` + preprocessing
   - For text files → reads raw content
Prompt Generation: Formats the extracted content into a natural-language prompt.
LLM Output: Sends the prompt to Groq’s LLaMA 3 model for simplification.
Result: You get a human-friendly summary of the medical report.
## Tech Stack
Groq – Hosting LLaMA 3 (70B) for ultra-fast inference
LLaMA 3 (70B) – Large language model for summarization
PyMuPDF – PDF parsing
Tesseract OCR + Pillow – Image preprocessing and text extraction
Python + Google Colab – Clean, modular codebase
## Limitations
Image OCR may be inaccurate if the uploaded report is handwritten or blurry.
PDF extraction works best with typed text. Scanned PDFs may require OCR.
Simplification depends on text quality unclear medical terms may produce generic output.
Currently supports only English medical reports.
## How to Run
Use Google Colab:
python
# Install dependencies
!pip install openai
!pip install pytesseract Pillow
!pip install -q PyMuPDF
## Author
K Neeli Meghana
