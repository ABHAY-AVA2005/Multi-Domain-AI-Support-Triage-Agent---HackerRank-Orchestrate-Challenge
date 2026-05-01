Here is your **final, clean, recruiter-grade README.md** — properly structured, concise, and high-impact. You can directly copy-paste this into your repo.

---

````md
# 🏆 Multi-Domain Support Triage Agent

AI-powered support triage system using **RAG + Gemini** that classifies, retrieves, and safely responds or escalates support tickets across multiple domains.

---

## 🚀 Quick Demo

```bash
cd code
python main.py --ticket "How do I reset my password?"
````

```bash
python main.py --batch
```

---

## 📌 Problem

Support tickets are often:

* Unstructured and ambiguous
* Spread across multiple domains
* Contain sensitive issues (fraud, billing, access)

The challenge is to:

* classify the request
* retrieve relevant information
* decide whether to reply or escalate
* generate safe, grounded responses

---

## 🧠 Solution

Built a **Multi-Domain AI Support Triage Agent** that:

* Classifies tickets (domain, intent, request type)
* Retrieves relevant documentation using **RAG**
* Applies **multi-layer safety checks**
* Decides **Reply vs Escalate**
* Generates **grounded responses (no hallucinations)**

---

## 🔄 Pipeline

1. **Ticket Classification (Gemini)**
2. **Embedding + Retrieval (FAISS)**
3. **Safety & Risk Check**
4. **Decision Engine (Reply / Escalate)**
5. **Response Generation (RAG)**
6. **Output (CSV + Logs)**

---

## ⚙️ Tech Stack

* **LLM**: Google Gemini
* **RAG**: FAISS + SentenceTransformers
* **Language**: Python
* **Data Processing**: Pandas, NumPy
* **Terminal UI**: Rich, Colorama, TQDM
* **Config Management**: python-dotenv

---

## 🚀 Features

* 🌐 Multi-domain support (HackerRank, Claude, Visa)
* 🧠 Intelligent classification & intent detection
* 🔍 RAG-based grounded responses
* 🛡️ Multi-layer safety system
* ⚠️ Context-aware escalation logic
* 🎨 Rich terminal UI
* 📊 Incremental CSV saving (fault-tolerant)
* 📈 Real-time processing feedback

---

## 🛠️ Installation

```bash
pip install -r code/requirements.txt
cp code/.env.example code/.env
```

Add your API key in `.env`:

```bash
GEMINI_API_KEY=your_api_key_here
```

Build index:

```bash
cd code
python main.py --rebuild-index
```

---

## 🎯 Usage

### Batch Mode

```bash
python main.py --batch
```

### Single Ticket

```bash
python main.py --ticket "Your query here"
```

### Interactive Mode

```bash
python main.py --interactive
```

---

## 📊 Output Format

```csv
sequence_order,ticket_id,timestamp,status,product_area,response,justification,request_type
```

---

## 🛡️ Safety & Escalation

* Prompt injection detection
* Harmful content filtering
* High-risk keyword detection (fraud, billing, security)
* Low-confidence escalation
* Strict **grounded responses only** (no hallucinations)

---

## 📁 Project Structure

```
hackerrank-orchestrate-may26/
├── README.md
├── AGENTS.md
├── problem_statement.md
├── evalutation_criteria.md
├── TECHNICAL_DOCUMENTATION.md
├── code/
│   ├── main.py
│   ├── requirements.txt
│   ├── .env.example
│   └── faiss_index/
├── data/
├── support_tickets/
```

---

## 🧠 Architecture Overview

* **RAG Pipeline** with FAISS vector search
* ~18K+ knowledge chunks indexed
* Gemini-powered classification & generation
* Modular pipeline (classification → retrieval → safety → response)

---

## 📈 Performance

* ⚡ ~6 tickets/min (API-limited)
* 🔍 Sub-second retrieval (FAISS)
* 📊 Scalable to large datasets
* 🛡️ Fault-tolerant with incremental saving

---

## 🧪 Testing

```bash
python main.py --ticket "test query"
python main.py --batch
python main.py --interactive
```

---

## 🐛 Troubleshooting

**API quota exceeded**
→ Wait or upgrade plan

**Index missing**

```bash
python main.py --rebuild-index
```

**Permission error**
→ Close files using `output.csv`

---

## 🏆 Competition

Built for **HackerRank Orchestrate Challenge**

✔️ Uses only provided corpus
✔️ No hallucinated responses
✔️ Proper escalation logic
✔️ Exact output schema compliance

---

## 📌 Key Learnings

* AI systems require **pipeline design**, not just prompts
* Retrieval + safety + decision-making = real intelligence
* Knowing **when NOT to answer** is critical
* Building from scratch gives better control than black-box frameworks

---

## 🔗 Author

**Abhay Varshit Aripirala**
B.Tech CSE | AI & Systems Enthusiast

---

⭐ If you found this interesting, feel free to star the repo!

```

---

# 🔥 This Version Fixes Everything

✔ Clean structure  
✔ No repetition  
✔ High recruiter readability  
✔ Strong technical signal  
✔ Proper flow (Demo → Problem → Solution → Tech → Depth)  

---

If you want next level:

👉 I can add:
- badges (stars, license, tech)
- architecture image
- demo GIF  
- recruiter-optimized highlights  

Just say **“make it elite README”** 🚀
```
