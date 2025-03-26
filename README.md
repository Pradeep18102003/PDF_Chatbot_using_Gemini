# 📚 Chat with PDF using Gemini

An interactive PDF chatbot application built with Streamlit and Google Gemini API. This project allows users to upload PDF documents and ask questions based on the content. The chatbot uses Google Gemini's embedding and chat model to provide detailed responses from the uploaded documents.

## 🚀 Features

- Upload and process multiple PDF files.
- Ask questions related to the content of the PDF.
- Uses Google Gemini API for embeddings and question answering.
- Efficient text chunking for handling large PDF files.
- Local FAISS index for fast and accurate document retrieval.

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Create a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the project root directory and add your Google Gemini API key:

```
GOOGLE_API_KEY=your_google_api_key
```

### 5. Run the Application

```bash
streamlit run app.py
```

## 📄 Project Structure

```
├── .gitignore
├── README.md
├── app.py
├── requirements.txt
└── .env
```

## 📊 How It Works

1. **Upload PDFs**: Users can upload one or multiple PDF files.
2. **Process PDFs**: Extracts text from PDFs and splits them into manageable chunks.
3. **Create Vector Store**: Uses Google Gemini embeddings to create a FAISS vector store for similarity search.
4. **Ask Questions**: Users can ask questions, and the app retrieves the most relevant text chunks and generates answers using the Gemini model.

## 🧰 Technologies Used

- Python
- Streamlit (for the web interface)
- Google Gemini API (for embeddings and chat)
- FAISS (for building and querying the vector store)
- LangChain (for managing the conversational chain)
- PyPDF2 (for extracting text from PDFs)
- python-dotenv (for handling environment variables)

## 📌 Notes

- Ensure you have a valid Google Gemini API key.
- The app saves the FAISS index locally to "faiss_index".

## 📧 Contact
- If you have any questions or feedback, feel free to reach out via email: pradeep18kumar10@gmail.com  
- LinkedIn: [Pradeep Kumar](https://www.linkedin.com/in/pradeep-kumar-bba090320/)


---

Enjoy interacting with your PDFs seamlessly using the power of AI! 🤖

