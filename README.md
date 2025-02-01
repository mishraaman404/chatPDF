# Name: Aman Mishra
# link to repo: https://github.com/mishraaman404/chatPDF.git

# Content of the project

### Concise Summary: PDF-Based Q&A System 
- **Purpose**: Enables users to upload PDFs and ask questions, providing accurate answers with source references.  
- **Key Features**:  
  - Extracts text from PDFs and splits it into chunks for efficient processing.  
  - Embeds text using OpenAI embeddings and stores it in a Chroma vector database.  
  - Answers questions via a chatbot powered by LangChain’s retrieval-based chain.  
- **User Interaction**: Chat interface for question answering, ensuring responses include cited sources.  
- **Tech Stack**: Python, LangChain, Chainlit, OpenAI API, PyPDF2, dotenv, Chroma.  
- **Use Cases**: Query large PDFs like research papers, contracts, or manuals interactively.  

A sleek, AI-driven tool for extracting and querying document insights.

# langchain-openai-chainlit
Chat with your pdfdocuments using Openai model, LangChain and Chainlit.  

- Upload a document
- Create a chatbot app with the ability to display sources used to generate an answer
---

## Steps to Replicate 

1. Fork this repository and create a codespace in GitHub as I showed you in the youtube video OR Clone it locally.
```
git clone https://github.com/mishraaman404/chatPDF.git
cd langchain-openai-chainlit
```
make an file in the directory named .env and put the below mentioned content.
   ```
   OPENAI_API_KEY=your_openai_api_key
   ```

2. Create a virtualenv and activate it
   ```
   python -m venv virtual_environment_name
   virtual_environment_name\Scripts\activate.bat
   ```

4. Run the following command in the terminal to install necessary python packages:
   ```
   pip install -r requirements.txt
   ```

5. Run the following command in your terminal to start the chat UI:
   ```
   chainlit run pdf_qa.py -w
   ```
---


