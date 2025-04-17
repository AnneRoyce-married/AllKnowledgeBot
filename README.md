# AIKnowledgeBot

+----------------------------------------+
| 📂 Upload File                         |
| [Choose File] [Upload]                |
+----------------------------------------+

💬 Ask a Question:
[ How does this policy handle refunds? ] (Submit)

🧠 GPT Answer:
> The policy allows refunds within 30 days...

[Ask Another Question]
+-------------------------------------------------------------------------+
Features

📂 Upload .txt files (PDF support coming soon)

💬 Ask natural language questions about the file's content

🔍 AI finds relevant context using semantic search

🧠 GPT generates accurate answers based on context

🧾 Simple web UI with chat-style Q&A interface

+------------------------------------------------+

📂 How It Works
User uploads a .txt file.

The backend extracts and splits text into chunks.

Each chunk is converted into a vector using OpenAI's Embedding API.

When the user asks a question:

The question is also embedded.

The most relevant chunks are selected using cosine similarity.

A prompt is created using these chunks + the question.

The prompt is sent to GPT (gpt-3.5-turbo or gpt-4).

GPT returns an answer based on the context and question.

