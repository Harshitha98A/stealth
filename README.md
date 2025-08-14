# 🎓💬 Soch with the Coach — Hybrid RAG Career Guidance Chatbot

One-line: 🚀 A hybrid static + RAG Streamlit chatbot that delivers career guidance & motivational advice to students 📚 — powered by curated Edexlive columns by Adarsh Benakappa Basavaraj 📝, with transparent citations 🔍 and premium feature gating 🔒.
(Think of it as your personal career coach who never needs coffee… but runs entirely on Python.) 🐍☕

## ✨ Key Features

🧠 Hybrid Knowledge → Instant predefined Q&A ⚡ plus RAG via LlamaIndex VectorStoreIndex for deeper answers.
(Because sometimes the answer is in the PDF… and sometimes in my “big brain” cache.)

📜 Source-Aware Outputs → Displays citations (article titles/links) under each answer.
(No “my uncle told me this” facts — only verified sources.)

🔒 Paid Gating → Unlock premium questions for paid users.
(Paywall: where curiosity meets capitalism.) 💸

⚡ Fast UX → Cached indexing, sidebar quick questions, and compact response mode.
(Less waiting, more wisdom.)

📦 Portable UI → Single-file Streamlit app; bring your own PDFs.
(B.Y.O.P — Bring Your Own PDFs.)

## 🛠 Tech Stack

🎨 UI: Streamlit (because CSS and I are “taking a break”)

🤖 LLM: OpenAI GPT (via LlamaIndex)

🔍 Retrieval: LlamaIndex VectorStoreIndex

📂 Loaders: PDFReader (Edexlive PDFs)

🐍 Lang: Python (the only snake that helps with your career)

## ⚙️ How It Works

1️⃣ Ingest PDFs (Edexlive education columns) 📄
2️⃣ Index with LlamaIndex → embeddings → VectorStoreIndex 🗄
3️⃣ Query Engine → retrieves top chunks & crafts prompt for GPT 🤖
4️⃣ Hybrid Layer → static answers for FAQs, fallback to RAG when needed 🔄
5️⃣ Citations rendered under each response 📜 + paid gating for premium queries 💳

(Basically: PDFs go in, smart answers come out, and I take all the credit.)

### 💻 Run Locally
pip install streamlit llama-index openai
export OPENAI_API_KEY="your_api_key"
streamlit run test_app3.py

📂 Configure Content

📥 Place PDFs (Edexlive by Adarsh Benakappa Basavaraj) in a folder → point the app to it in the UI/ENV.

🛠 Adjust paid question list, static Q&A, and sidebar quick questions in test_app3.py.

(Yes, you can sneak in your own PDFs — I won’t tell.) 🤫

### 🎯 Demo Tips

📄 Preload 3–5 edexlive PDFs and ask: “How to build consistency for exam prep?”

🔒 Show a premium question to demo paid gating, then a RAG question to show citations.

#### (Pro tip: When they say “Wow!”, casually say “Yeah, I built that over a weekend”… even if it took three.) 😏
