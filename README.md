# Chat PDF with Gemini  

This Streamlit application leverages Google's GenerativeAI service (Gemini) to enable users to ask questions and get answers from uploaded PDF documents.

## Run on Streamlit  

You can run this app on Streamlit Server: [Chat with Multiple PDF](https://chat-multiple-documents.streamlit.app)

## 1. Features

- **PDF Upload:** Upload multiple PDF documents for analysis.
- **Conversational Interface:** Ask questions in natural language related to the uploaded PDFs.
- **AI-powered Information Retrieval:** Gemini analyzes the PDFs and retrieves relevant information to answer your questions.
- **Context Awareness:** The model considers the entire context of the PDFs when answering your questions.

## 2. Requirements

- Python 3.x
- Streamlit (`pip install streamlit`)
- `PyPDF2` library (`pip install PyPDF2`)
- Langchain libraries (`pip install langchain langchain-google-genai`)
- Google Cloud Project with GenerativeAI API enabled ([https://cloud.google.com/ai/generative-ai](https://cloud.google.com/ai/generative-ai))
- `dotenv` library (`pip install python-dotenv`)

## 3. Setup

1. Create a virtual environment (recommended): `python -m venv venv`
2. Activate the environment: `source venv/bin/activate` (Windows: `venv\Scripts\activate`)
3. Install dependencies: Refer to the requirements section and install the necessary libraries.
4. Create a `.env` file in the project directory:
   - Add `GOOGLE_API_KEY=<YOUR_API_KEY>` (replace with your GenerativeAI API key)

## 4. Running the App

1. Open a terminal in the project directory.
2. Run the app: `streamlit run app.py`
3. Access the app in your web browser at http://localhost:8501.

## 4. Usage

1. Upload one or more PDF documents using the file uploader in the sidebar.
2. Click the "Submit & Process" button to generate a vector index from the uploaded PDFs.
3. In the main area, type your question related to the uploaded documents.
4. Click "Enter" or submit the question to receive a response from the AI model.

## 5. Disclaimer

- This is a basic example using a free-tier API. The accuracy and detail of answers may vary.
- Consider the limitations of natural language processing and the quality of the uploaded PDFs for the best results.

## Note

- This README assumes you have completed initial setup and configured your Google Cloud Project with the GenerativeAI API.