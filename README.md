# Working

<p align="center">
  <img src="https://github.com/user-attachments/assets/9c7d701b-d680-49d6-8c5e-b7c4fb4a92fa">
</p>

---



```mermaid
flowchart TD
    A[📤 Upload PDF (Gradio UI)] --> B[📄 Extract Text using PyPDF]
    B --> C[✂️ Chunk Text into Segments]
    C --> D[🔢 Embed Chunks using Sentence Transformers]
    D --> E[📦 Store Embeddings in Pinecone]
    E --> F[❓ User Asks a Question]
    F --> G[🔍 Retrieve Relevant Chunks (Pinecone)]
    G --> H[🧠 Build Prompt with Retrieved Context]
    H --> I[💬 Generate Answer using FLAN-T5]

