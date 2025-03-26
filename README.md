# **Know-Your-State With AI** 💬📚  

This Streamlit-based web application allows users to interact with multiple PDF files by uploading them and asking questions. The app extracts text from PDFs, processes it using embeddings from Google's Generative AI (Gemini model), and answers questions based on the PDF content.

---

## **Features**  
- **PDF Upload and Processing**: Upload multiple PDFs and extract their text.  
- **Text Splitting and Chunking**: Splits large text content into manageable chunks for effective querying.  
- **Vector Store with FAISS**: Saves text chunks as embeddings for efficient similarity search.  
- **Conversational AI**: Uses Google's Gemini-based Generative AI model to answer user queries with detailed context-based replies.  
- **User-Friendly Interface**: Built using Streamlit for easy interaction.  

---

## **Tech Stack**  
- **Python Libraries**:  
  - `streamlit` – For building the web app UI  
  - `PyPDF2` – For PDF text extraction  
  - `langchain` – For prompt creation, embeddings, and conversational chains  
  - `FAISS` – For vector-based similarity search  
  - `dotenv` – To load environment variables  
  - `google.generativeai` – For embeddings and chat model (Gemini)  

---

## **How to Run Locally**  

### **1. Clone the Repository**  
```bash  
git clone <repository-url>  
cd <repository-folder>  
```  

### **2. Set Up Virtual Environment and Install Requirements**  
```bash  
python -m venv myenv  
source myenv/bin/activate  # For Linux/Mac  
myenv\Scripts\activate     # For Windows  
pip install -r requirements.txt  
```  

### **3. Configure API Key**  
- Create a `.env` file in the root directory and add your **Google Generative AI API Key**:  
  ```  
  GOOGLE_API_KEY=your_api_key_here  
  ```  

### **4. Run the Application**  
```bash  
streamlit run app.py  
```  

---

## **How It Works**  
1. **PDF Upload**:  
   - Upload multiple PDF files via the sidebar.  
   - Click **Submit & Process** to extract and process the text.  

2. **Ask a Question**:  
   - Enter your question in the text box on the main page.  
   - The app will search the processed PDF content and provide a detailed, context-based answer.  

---

## **Project Structure**  
- `app.py`: The main application logic (provided in the code).  
- `.env`: Environment variables for API key storage.  
- `requirements.txt`: Dependencies required to run the project.  

---

## **Future Enhancements (Optional)**  
- Add support for additional file formats (e.g., DOCX, TXT).  
- Improve the UI/UX for better user experience.  
- Implement additional models for embeddings or QA chains.  

---

## **Acknowledgments**  
This project leverages cutting-edge tools and libraries from the AI/ML ecosystem, particularly Google's Generative AI and LangChain for conversational capabilities.

