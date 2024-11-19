## Project Link
[https://chatwithyourdata.netlify.app/](https://chatwithyourdata.netlify.app/)


# Chat with Data

This project, **Chat with Data**, is a powerful tool for interacting with various types of data sources. Users can upload their data in different formats or connect to external databases and websites for meaningful and interactive conversations. It contains four main modules:

1. **Chat with PDF**  
2. **Chat with CSV**  
3. **Chat with Databases**  
4. **Chat with Website**  
---
https://github.com/user-attachments/assets/3db76e5a-de09-45df-9808-a5e21a25fe91





## Features

### 1. Chat with PDF 📑 
- Users upload a PDF document.  
- The system extracts the content from the PDF and allows users to ask questions based on the document's content.  
- Supports multi-page PDFs and handles scanned or searchable text.

### 2. Chat with CSV 📄 
- Users upload a CSV file.  
- The system parses the file, enabling users to query the data.  
- Provides capabilities for summarization, filtering, and specific data retrieval.  

### 3. Chat with Databases  🗄️
- Users connect their local databases.  
- Supported databases include MySQL, PostgreSQL, SQLite, and others via provided credentials:  
  - **User ID**  
  - **Password**  
  - **Host**  
  - **Port**  
  - **Database Name**  
- Once connected, users can query the database using plain English commands.

### 4. Chat with Website  🌐 
- Users enter a website URL to interact with.  
- Multiple website URLs can be provided.  
- Extracts meaningful data from the website, enabling users to ask questions based on the site's content.  

---
# Workflow Explanation
![rag](https://github.com/user-attachments/assets/f8350b96-402e-45ee-97cd-379a3134accf)
---

## Steps:

### 1. **User Input (Prompt)**  
   - The user provides a query or a prompt.  
   - This input is processed by a **Question Encoder**, which converts the text into a vector (a numerical representation of the input).

---

### 2. **Document/Data Encoding**  
   - The system processes the documents or stored data using a **Context Encoder**.  
   - The Context Encoder transforms the documents into vectors that represent their meaning in a machine-readable format.  
   - These encoded vectors are stored in a **Vector Database (Vector DB)** for easy retrieval.

---

### 3. **Retrieving Relevant Information**  
   - The system compares the vector from the user’s question with the vectors stored in the database.  
   - It retrieves the most relevant context or data based on similarity.

---

### 4. **Combining Prompt and Context**  
   - The retrieved context is combined with the original query (prompt).  
   - This step ensures the response is enriched with relevant information from the database.

---

### 5. **Response Generation**  
   - The enriched input (prompt + context) is passed to a chatbot or a response generation model.  
   - The chatbot generates a response tailored to the user’s query based on the retrieved context.

---

## Key Features:
- **Efficient Retrieval**: The system uses vector-based matching to find relevant information quickly.  
- **Flexible Understanding**: Even if the query wording differs from the stored data, the vector representation ensures the correct match.  
- **Accurate Responses**: By combining user input with retrieved context, the system provides meaningful and precise answers.

---

### Workflow Diagram:
Refer to the workflow diagram for a visual representation of the process.

## Requirements  

- Python 3.8 or later  
- Necessary libraries (install via `requirements.txt`):  
  ```bash
  pip install -r requirements.txt
