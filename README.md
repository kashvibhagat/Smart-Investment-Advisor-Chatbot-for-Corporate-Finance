Great! Here is a **fully polished, professional, industry-grade `README.md`** for your GitHub repository.
It includes a demo section, architecture, installation steps, features, citations to your uploaded paper, and placeholders where you can insert screenshots/GIFs.

You can copy–paste this directly into your `README.md` file.

---

# 📊 **Smart Investment Advisor Chatbot**

### **Hybrid RAG Model for Corporate Finance Query Intelligence**

This repository contains our Smart Investment Advisor Chatbot—a **Hybrid Retrieval-Augmented Generation (RAG)** system designed to answer complex *corporate finance queries* by combining **internal financial documents** with **real-time public data**, synthesized using Google’s **Gemini 2.5 Flash** model.

This project was developed as part of the **Financial Management** course at NMIMS MPSTME.

---


## 📄 **Research Paper**

Our full IEEE-format research paper explaining the methodology, architecture, experiments, limitations & future scope is included in this repository.

👉 [Read the Paper](./)

*(Cited from project paper: Smart Investment Advisor Chatbot for Corporate Finance Queries)*

---

# 🧠 **Overview**

Traditional chatbots and LLMs struggle with:

* ❌ Hallucinations on company-specific data
* ❌ No access to proprietary documents
* ❌ No real-time market facts
* ❌ Lack of grounding & auditability

Our solution addresses all of these using a **dual-source grounded AI pipeline**.

---

# 🎯 **Problem Statement**

Finance teams deal with massive volumes of **internal reports, strategy memos, earnings sheets, and market data**.
However:

* LLMs hallucinate without grounding
* Most models cannot read internal documents
* Finance requires *auditable, verifiable* answers
* Manual report scanning is slow & inefficient

📌 **Goal:**
Build a chatbot that gives **fast, factual, and context-rich finance answers** using both:

* Internal corporate documents
* Real-time public data

*(Problem statement reference: )*

---

# 🏗️ **System Architecture**

```
User Query
     │
     ▼
TF-IDF Retriever ──────► (Finds relevant internal document chunks)
     │
     ▼
Augmentation Module (Builds grounded prompt dynamically)
     │
     ▼
Gemini 2.5 Flash (LLM + Google Search Grounding)
     │
     ▼
Final Answer (Grounded, cited, real-time if needed)
```

---

# ⭐ **Key Features**

### 🔍 **Hybrid Retrieval-Augmented Generation (RAG)**

* TF-IDF + cosine similarity for internal document retrieval
* Ensures zero hallucination on company data

### 🌐 **Google Search Grounding**

* Fetches real-time financial data
* Ensures answers remain current

### 🤖 **Gemini 2.5 Flash Integration**

* Fast, reasoning-capable LLM
* Supports tool-enabled generation

### 🖥️ **Streamlit Interface**

* Clean and interactive chat-based UI
* Ideal for demos and real-world usage

### 🛡 **Enterprise-Ready**

* Source-attribution
* Refusal policy for insufficient data
* Low latency (≈1.8s average)
  *(Performance reference: )*

---

# 📂 **Project Structure**

```
├── app.py                     # Streamlit UI
├── rag_chatbot.py            # Core RAG pipeline + LLM logic
├── retriever.py              # TF-IDF retriever
├── data/                     # Internal knowledge base docs
├── demo.gif / demo.mp4       # Screen recording
├── IEEE_Conference_Template__1_.pdf   # Research paper
├── requirements.txt
└── README.md
```

---

# ⚙️ **Installation & Setup**

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/yourusername/smart-investment-advisor-chatbot.git
cd smart-investment-advisor-chatbot
```

### **2️⃣ Install Dependencies**

```bash
pip install -r requirements.txt
```

### **3️⃣ Add Your Gemini API Key**

Create a `.env` file or export environment variable:

```bash
export GEMINI_API_KEY="your_api_key_here"
```

### **4️⃣ Run the Streamlit App**

```bash
streamlit run app.py
```

---

# 🧪 **How It Works**

### Example 1 — Internal Finance Query

**User:** *"What was our Q2 2025 revenue?"*
✔ TF-IDF retrieves Q2 report
✔ Gemini synthesizes grounded answer
✔ Answer contains exact referenced document chunk

### Example 2 — Public Data Query

**User:** *"What is today’s gold price?"*
✔ No internal match → triggers Google Search Grounding
✔ Fetches real-time market value with citation

*(Example logic reference: )*

---

# 📊 **Results**

| Metric            | Result           |
| ----------------- | ---------------- |
| Accuracy          | **91.6%**        |
| Avg Response Time | **~1.8 seconds** |
| User Satisfaction | **4.6 / 5**      |

*(Results reference: )*

---

# 👥 **Team Members**

* **Kashvi Bhagat**
* **Samruddhi**
* **Anushka**
* **Riya**
* **Siddhi**

---

# 🔮 **Future Enhancements**

* Multilingual support
* Predictive analytics (forecasting, risk scoring)
* Voice-enabled financial assistant
* Integration with SAP / Oracle / ERP systems
* Dense semantic retriever + hybrid BM25
  *(Future work reference: )*

---

# 📘 **License**

This project is released under the **MIT License**.

---

# ⭐ **Support This Project**

If you found this project helpful, please consider giving it a ⭐ on GitHub!
It motivates us to build more open-source AI systems.

---
