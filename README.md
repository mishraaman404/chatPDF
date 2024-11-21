# langchain-openai-chainlit
Chat with your documents (pdf, csv, text) using Openai model, LangChain and Chainlit.  
In these examples, we’re going to build an chatbot QA app. We’ll learn how to:

- Upload a document
- Create vector embeddings from a file
- Create a chatbot app with the ability to display sources used to generate an answer
---

## Steps to Replicate 

1. Fork this repository and create a codespace in GitHub as I showed you in the youtube video OR Clone it locally.
```
git clone https://github.com/mishraaman404/chatPDF.git
cd langchain-openai-chainlit
```

   ```
   OPENAI_API_KEY=your_openai_api_key
   ```

2. Create a virtualenv and activate it
   ```
   python3 -m venv .venv && source .venv/bin/activate
   ```

   If you have python 3.11, then the above command is fine. But, if you have python version less than 3.11. Using conda is easier. First make sure that you have conda installed. Then run the following command.
   ```
   conda create -n .venv python=3.11 -y && source activate .venv
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