# Chat with Data

This project, **Chat with Data**, is a powerful tool for interacting with various types of data sources. Users can upload their data in different formats or connect to external databases and websites for meaningful and interactive conversations. It contains four main modules:

1. **Chat with PDF**  
2. **Chat with CSV**  
3. **Chat with Databases**  
4. **Chat with Website**  

---

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

## Requirements  

- Python 3.8 or later  
- Necessary libraries (install via `requirements.txt`):  
  ```bash
  pip install -r requirements.txt
