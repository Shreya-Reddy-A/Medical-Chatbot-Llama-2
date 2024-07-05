# Medical-Chatbot

This project offers a comprehensive medical chatbot solution. Integrated seamlessly with ChainLit, it provides an easy-to-use chat interface powered by the LLAMA-2 language model renowned for its natural language processing capabilities. The chatbot efficiently retrieves and delivers precise information from a structured knowledge base stored in PDF documents, making it adept at handling complex medical queries with ease.

![Screenshot (226)](https://github.com/Shreya-Reddy-A/Medical-Chatbot-Llama-2/assets/122392746/bdc204f8-b988-4e0a-9590-129287aa0d60)

# Features
  - **Question Answering:** System responds to medical queries using pre-processed medical documents.
  - **Interactive Chat Interface:** Users interact via ChainLit-powered interface
  - **Vector Store Creation and Data Ingestion:** A script to ingest and preprocess PDF documents, creating a searchable vector store for the knowledge base.

# Getting Started
To get started follow these steps:

1. **Clone the Repository**:
   - Clone this repository to your local machine.
     ```
     git clone https://github.com/Shreya-Reddy-A/Medical-Chatbot-Llama-2.git
     ```

3. **Install Dependencies**:
   - Navigate into the cloned directory and install the necessary dependencies.
     ```
     cd Medical-Chatbot-Llama-2
     pip install -r requirements.txt
     ```
5. **Pdf data:**
   - Place medical PDF documents in the data/ directory.
  
6. **Download the model:**
   - Obtain the ```llama-2-7b-chat.ggmlv3.q8_0.bin``` file and place it in the project directory.
   
7. **Data setup:**
   - Run the ingestion script to preprocess the documents and create the vector store.
     ```
     python ingest.py
     ```
8. **Running the chatbot:**
   - Start the chatbot interface
     ```
     chainlit run model.py -w
     ```
7. Enter your medical query and the chatbot will provide answers sourced from the knowledge base.

# Dependencies
  - Langchain
  - ChainLit
  - Hugging Face Transformers
  - FAISS
