# Retrival-QA
This project is a Retrieval-Augmented Question Answering (QA) application that uses OpenAI’s language model in combination with FAISS for fast and accurate document-based search. It allows users to ask questions related to their own data and receive meaningful answers, along with the sources that support those answers.

Wrote by me! Edited by AI 😉 
📚 Project Title: Retrieval QA with FAISS and OpenAI

🔍 Description
This project is a question-answering app built using:

FAISS (Facebook AI Similarity Search) for fast and efficient document search

OpenAI's LLM (GPT) to generate answers based on retrieved content

LangChain to connect the retriever and LLM into a single pipeline

Streamlit for the interactive user interface

The app lets users ask questions based on custom documents, and it provides answers along with the source documents used to generate those answers.

🧠 How It Works (Brief Workflow)
Documents are split into chunks and converted to embeddings.

The embeddings are stored in a FAISS vector store (faiss_store_openai.pkl).

When a user enters a question:

The retriever searches for the most relevant chunks.

Those chunks are passed to the LLM via LangChain.

The LLM generates an answer based on the retrieved content.

The app displays the answer and the sources.

🚀 Technologies Used
-Python
-OpenAI API
-FAISS
-LangChain
-Streamlit

Pickle (for saving vector store)

🛠️ How to Run
pip install -r requirements.txt
streamlit run app.py