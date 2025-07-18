# KS_RAG_FAQ_CHATBOT
A Retrieval-Augmented Generation (RAG) based chatbot for answering FAQs about Knowledge Streams courses.
This chatbot uses ChromaDB for vector storage, Sentence Transformers for embeddings, and OpenAI GPT models (or other LLMs) for generating context-aware responses.

📌 Key Features
✅ Context-Aware Responses – Answers based on real course data
✅ RAG Pipeline – Combines semantic search with LLM for accuracy
✅ ChromaDB for Vector Storage – Persistent, fast, and lightweight
✅ Custom Knowledge Base – Uses knowledge_streams_courses.csv
✅ Streamlit UI – Interactive user interface for easy querying

📂 Project Structure
bash
Copy
Edit
KS_RAG_FAQ_CHATBOT/
│
├── data/
│   └── knowledge_streams_courses.csv     # Knowledge base file
│
├── app/
│   ├── embeddings.py                     # Generate embeddings & store in ChromaDB
│   ├── retriever.py                      # Query and retrieve relevant context
│   ├── generator.py                      # LLM response generator
│   ├── ui.py                             # Streamlit interface
│
├── main.py                               # Complete end-to-end chatbot
├── requirements.txt                      # Dependencies
└── README.md                             # Documentation
⚙️ Tech Stack
Language: Python 3.8+

Libraries:

pandas – For CSV data handling

sentence-transformers – Text embeddings

chromadb – Vector database

openai – LLM integration

streamlit – Web UI

Model: all-MiniLM-L6-v2 (fast & lightweight)

Deployment Options: Local / Streamlit Cloud / Hugging Face Spaces

