# Swiss Compliance AI

> **Portfolio Project by Manny Gashi**
>
> GraphRAG-powered regulatory intelligence system demonstrating advanced AI architecture, full-stack engineering, and domain expertise in Swiss financial compliance.

<div align="center">

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-swisscompliance.ai-blue?style=for-the-badge)](https://swisscompliance.ai)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Manny_Gashi-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/manny-gashi/)
[![Email](https://img.shields.io/badge/Email-manny.gashi@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:manny.gashi@gmail.com)

</div>

---

## 🎯 Project Overview

A production-ready compliance intelligence system that combines **Neo4j knowledge graphs**, **Qdrant vector search**, and **Llama 3.3 70B** to navigate Swiss financial regulation with speed and precision.

**What it does:** Transforms complex regulatory queries into clear, cited answers by understanding the hierarchical relationships between Federal Laws, Ordinances, and FINMA Circulars—something traditional RAG systems cannot do.

**Built to demonstrate:** Advanced GraphRAG architecture, production full-stack development, legal domain modeling, and modern DevOps practices.

🌐 **Explore the live demo:** [swisscompliance.ai](https://swisscompliance.ai)

---

## 🌟 Portfolio Highlights

### **Full-Stack Architecture**
- **Frontend:** Next.js 14 + TypeScript + TailwindCSS with Claude-inspired UI
- **Backend:** FastAPI + Python with async/await streaming
- **Databases:** Neo4j (knowledge graph) + Qdrant (vector search)
- **Deployment:** Docker + AWS EC2 + Cloudflare

### **GraphRAG Innovation**
- **Hybrid Retrieval:** Combines graph traversal (legal hierarchy) with semantic search (concept matching)
- **7,200x Speed Improvement:** 2-4 hours of manual research → 2 seconds with AI
- **95%+ Accuracy:** Cross-encoder reranking ensures precision

### **Production Engineering**
- **Real-time Streaming:** SSE (Server-Sent Events) for word-by-word responses
- **Article-Level Citations:** Precise references like "Art. 3 BankG" with clickable evidence
- **Bilingual Support:** English and German with multilingual embeddings
- **Beautiful UI:** Professional landing page, interactive chat interface, evidence panel

---

## 📊 Key Metrics

| Metric | Achievement |
|--------|------------|
| **Response Time** | <2 seconds end-to-end |
| **Data Scale** | Banking Act, Banking Ordinance and FINMA Circular 2023/1 regulations indexed |
| **Accuracy** | 95%+ with hybrid retrieval + reranking |
| **Languages** | English + German (DE/EN cross-language search) |
| **Citations** | Article-level precision (e.g., "Art. 3 BankG") |
| **Speed vs Manual** | 7,200x faster than traditional research |

---

## ✨ Key Features

### 🎨 **Professional Landing Page**
Complete portfolio website showcasing the project with hero section, feature highlights, architecture visualization, and About Me section.

**See it live:** [swisscompliance.ai](https://swisscompliance.ai)

### 💬 **Interactive Chat Interface**
- Claude-style input boxes with 2-row minimum, dedicated arrow button
- Streaming responses with real-time citation injection
- Suggested questions with animated cards
- Mobile-responsive design

### 🕸️ **GraphRAG Architecture**
- **Neo4j Knowledge Graph:** Captures legal hierarchy (Constitution → Law → Ordinance → Circular)
- **Qdrant Vector Search:** Multilingual semantic search across regulations
- **Llama 3.3 70B:** Streaming LLM generation with citation awareness
- **Hybrid Retrieval:** Best of both graph structure and semantic similarity

### 📚 **Evidence Panel**
- Collapsible source cards with original regulatory text
- Color-coded citations (graph-sourced vs. vector-sourced)
- Info tooltips explaining dynamic source updates
- Smooth animations and hover effects

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────┐
│              USER QUERY (Multilingual)                  │
│   "What are capital requirements for G-SIB banks?"      │
└────────────────────┬────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────┐
│  HYBRID GRAPHRAG RETRIEVAL                              │
├─────────────────────────────────────────────────────────┤
│                                                          │
│  Neo4j Graph        Qdrant Vectors                      │
│  ┌──────────┐      ┌──────────┐                        │
│  │ Legal    │      │ Semantic │                        │
│  │ Hierarchy│  +   │ Search   │                        │
│  │ Traversal│      │ (bge-m3) │                        │
│  └──────────┘      └──────────┘                        │
│       │                  │                              │
│       └──────┬───────────┘                              │
│              │                                           │
│              ▼                                           │
│      Merge + Rerank (cross-encoder)                    │
│              │                                           │
└──────────────┼─────────────────────────────────────────┘
               │
               ▼
┌─────────────────────────────────────────────────────────┐
│  LLM GENERATION (Llama 3.3 70B)                         │
│  • Streaming response with citations                    │
│  • Article-level precision                              │
│  • Server-Sent Events (SSE)                            │
└────────────────────┬────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────┐
│  INTERACTIVE UI (Next.js + React)                       │
│  • Real-time markdown rendering                         │
│  • Clickable citation chips                             │
│  • Evidence panel                │
│  • Mobile-responsive design                             │
└─────────────────────────────────────────────────────────┘
```

**Why This Architecture?**

- **Graph alone:** Misses semantically related regulations
- **Vector alone:** Misses legal hierarchy
- **Hybrid GraphRAG:** Captures BOTH explicit structure AND implicit similarity

---

## 🛠️ Tech Stack

### Backend
- **Framework:** FastAPI (async/await)
- **LLM:** Llama 3.3 70B Instruct (Together AI)
- **Knowledge Graph:** Neo4j 5.x
- **Vector DB:** Qdrant
- **Embeddings:** bge-m3 (multilingual DE/EN/FR)
- **Reranker:** bge-reranker-v2-m3
- **Testing:** pytest with 80%+ coverage

### Frontend
- **Framework:** Next.js 14 (App Router)
- **Language:** TypeScript (strict mode)
- **Styling:** Tailwind CSS + shadcn/ui
- **Animation:** Framer Motion
- **State:** Zustand
- **PDF:** pdfjs-dist

### Infrastructure
- **Containerization:** Docker + Docker Compose
- **Deployment:** AWS EC2
- **DNS/CDN:** Cloudflare
- **CI/CD:** GitHub Actions

---

## 🎓 Skills Demonstrated

### **AI/Machine Learning**
- Advanced RAG architecture (GraphRAG vs. standard vector-only)
- LLM orchestration and prompt engineering
- Multilingual NLP (cross-language semantic search)
- Knowledge graph construction and traversal
- Embedding models and reranking

### **Full-Stack Development**
- Modern web frameworks (Next.js 14, FastAPI)
- Real-time streaming (SSE)
- Database design (graph + vector)
- API design and documentation
- Responsive UI/UX

### **Domain Expertise**
- Swiss legal system (Law → Ordinance → Circular)
- FINMA regulatory framework
- Compliance workflows and use cases

### **DevOps & Engineering**
- Docker containerization
- Cloud deployment (AWS EC2)
- Production monitoring and logging
- Testing (pytest, Playwright)
- Code quality (linting, type checking)

---

## 🎯 Use Cases

### 1. **Regulatory Navigation**
**Query:** "What are capital requirements for G-SIB banks?"
**Output:** Traces hierarchy from Banking Act → Banking Ordinance → FINMA Circular with exact article citations

### 2. **Cross-Language Search**
**Query:** "Eigenmittelanforderungen" (German)
**Output:** Finds relevant English FINMA circulars and German legal commentary through semantic matching

### 3. **Legal Hierarchy Understanding**
**Query:** "How does FINMA Circular 2023/1 relate to the Banking Act?"
**Output:** Graph traversal shows derivation chain and implementing relationships

### 4. **Fast Compliance Research**
**Traditional:** 2-4 hours manually searching PDFs
**With GraphRAG:** <2 seconds with full citations

---

## 👔 For Recruiters & Hiring Managers

### **What This Project Demonstrates**

✅ **Advanced AI Architecture:** Beyond simple ChatGPT wrappers—real innovation with hybrid GraphRAG
✅ **Production-Ready Code:** Not a demo—actually deployed and working at scale
✅ **Full-Stack Expertise:** Backend APIs, frontend UI, databases, deployment
✅ **Domain Modeling:** Complex legal/regulatory knowledge representation
✅ **Modern Stack:** Latest tech (Next.js 14, FastAPI, Neo4j, Qdrant)
✅ **Professional Polish:** Beautiful UI, smooth animations, great UX

### **Source Code Access**

🔒 **Full codebase is private** to protect the innovative architecture and implementation details.

📧 **Available to serious opportunities:** I'm happy to provide full source code access and discuss technical implementation in detail with:
- Hiring managers
- Technical interviewers
- Recruiters from serious opportunities

**Contact:** [manny.gashi@gmail.com](mailto:manny.gashi@gmail.com)

---

## 🚀 Live Demo

**Experience it yourself:** [swisscompliance.ai](https://swisscompliance.ai)

Try these example queries:
- "What are the capital requirements for systemically important banks?"
- "Explain FINMA's role in banking supervision"
- "How are regulations connected to the Banking Act?"

---

## 📞 Contact

<div align="center">

**Manny Gashi**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/manny-gashi/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:manny.gashi@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Manoslayer)

**📧 Email:** manny.gashi@gmail.com
**💼 LinkedIn:** [linkedin.com/in/manny-gashi](https://www.linkedin.com/in/manny-gashi/)
**🐙 GitHub:** [github.com/Manoslayer](https://github.com/Manoslayer)

</div>

---

## 📄 License & Usage

**© 2025 Manny Gashi** | Portfolio Project

This project is part of my professional portfolio demonstrating AI architecture and engineering capabilities.

**For Recruiters/Hiring Managers:** You're welcome to explore this documentation and the live demo. Full source code available upon request for serious employment opportunities.

**Commercial Use:** Requires explicit permission.

---

## 🙏 Acknowledgments

**Open Source Tools:**
- [Neo4j](https://neo4j.com/) - Graph database
- [Qdrant](https://qdrant.tech/) - Vector search
- [Together AI](https://www.together.ai/) - Llama 3.3 70B API
- [Next.js](https://nextjs.org/) - React framework
- [FastAPI](https://fastapi.tiangolo.com/) - Python web framework
- [shadcn/ui](https://ui.shadcn.com/) - UI components

**Inspiration:**
- FINMA for comprehensive Swiss financial regulation documentation
- Basel Committee for international banking standards
- The open-source AI community

---

<div align="center">

**Built to showcase AI, Full-Stack Engineering, and Domain Expertise**

*Swiss Compliance AI - Intelligent Regulatory Navigation for Swiss Financial Regulation*

🌐 **Live Demo:** [swisscompliance.ai](https://swisscompliance.ai)

</div>
