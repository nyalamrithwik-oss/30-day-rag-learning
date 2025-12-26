# 🚀 30-Day RAG & MCP Learning Journey

[![Progress](https://img.shields.io/badge/Progress-26.7%25-blue.svg)](https://github.com/nyalamrithwik-oss/30-day-rag-learning)
[![Days](https://img.shields.io/badge/Days-8%2F30-green.svg)](https://github.com/nyalamrithwik-oss/30-day-rag-learning)
[![Time](https://img.shields.io/badge/Time-44%20hours-orange.svg)](https://github.com/nyalamrithwik-oss/30-day-rag-learning)
[![Goal](https://img.shields.io/badge/Goal-%243K--5K-success.svg)](https://github.com/nyalamrithwik-oss/30-day-rag-learning)

> **Master RAG systems and MCP development to generate $3K-5K in AI consulting revenue**

**Built by:** [Rithwik Nyalam](https://github.com/nyalamrithwik-oss) | **Location:** Karimnagar, Telangana, India

---

## 🎯 Mission

Transform from AI enthusiast to paid AI consultant in 30 days by mastering:
- ✅ **Retrieval-Augmented Generation (RAG)** systems
- 🚀 **Model Context Protocol (MCP)** development
- 💼 **Production-ready AI applications**

**End Goal:** $3,000-$5,000 in consulting revenue from AI projects

---

## 📊 Progress Overview

```
Week 1: ████████████████████  100% (7/7 days) ✅ RAG Fundamentals
Week 2: ████░░░░░░░░░░░░░░░░   14% (1/7 days) 🚀 MCP Development  
Week 3: ░░░░░░░░░░░░░░░░░░░░    0% (0/7 days) ⏳ Advanced Integration
Week 4: ░░░░░░░░░░░░░░░░░░░░    0% (0/9 days) ⏳ Production & Launch

Overall: ████░░░░░░░░░░░░░░░░  26.7% (8/30 days)
```

**Current Status:** Day 8 Complete | Week 2 Day 1 | Building MCP servers

---

## 📂 Project Repositories

### Week 1: RAG Fundamentals ✅ COMPLETE

#### 🔷 [Day 1-2: Basic RAG System](https://github.com/nyalamrithwik-oss/day1-basic-rag)
My first production RAG system - learned fundamentals of document retrieval and AI-powered Q&A

**What I Built:**
- Document loader (text/PDF files)
- Text splitter with chunking
- ChromaDB vector storage
- LangChain orchestration
- Basic Q&A interface

**Key Learnings:**
- RAG architecture (Retrieve → Augment → Generate)
- Vector embeddings and semantic search
- LangChain framework basics
- Virtual environment setup on Windows

**Tech Stack:** Python 3.10+, LangChain, OpenAI GPT-4, ChromaDB

**Stats:** ~150 lines of code | 8 hours | 1 test document

---

#### 🔷 [Day 3-5: Vector Database Comparison](https://github.com/nyalamrithwik-oss/day3-vector-comparison)
Deep dive into vector databases - compared 3 major options and implemented hybrid search with re-ranking

**What I Built:**
- ChromaDB implementation (local vector storage)
- Pinecone implementation (cloud-based, serverless)
- Weaviate implementation (GraphQL, objects)
- Hybrid search combining BM25 keyword + vector semantic search
- Cohere re-ranking for top 10 results

**Key Learnings:**
- Each vector DB has different strengths
- Hybrid search beats pure vector search
- Re-ranking dramatically improves accuracy
- Trade-offs: cost vs. performance vs. ease of use

**Performance:**
- ChromaDB: Fast, free, local
- Pinecone: Scalable, $0.096/1M queries
- Weaviate: GraphQL flexibility
- Hybrid + Re-rank: 95%+ accuracy

**Tech Stack:** Python, ChromaDB, Pinecone, Weaviate, Cohere API, BM25

**Stats:** ~400 lines of code | 16 hours | 3 databases compared

---

#### 🔷 [Day 6-7: Smart Knowledge Base](https://github.com/nyalamrithwik-oss/portfolio-project-1) ⭐ **PORTFOLIO PROJECT #1**
Production-ready RAG system with beautiful UI - my first complete AI application ready for clients

**What I Built:**
- Multi-format document support (PDF, TXT, DOCX, MD)
- Streamlit web interface with file upload
- Hybrid search (vector + keyword)
- Cohere re-ranking for accuracy
- Beautiful UI with progress indicators
- Source citations with relevance scores
- Error handling and validation

**Key Features:**
- 📄 Upload any document format
- 🔍 Ask questions in natural language
- 🎯 Get answers with source citations
- ⚡ Response time: < 5 seconds
- 📊 Search accuracy: 95%+

**Real-World Use Cases:**
- Corporate knowledge base
- Research paper Q&A
- Legal document analysis
- Technical documentation search

**Tech Stack:** Python 3.10+, Streamlit, ChromaDB, OpenAI GPT-4, Cohere API

**Stats:** ~500 lines of code | 20 hours | 4 file formats | Deployment-ready

**Demo:** Fully functional web app with professional UI

---

### Week 1 Summary

**Achievements:**
- ✅ Built 3 complete RAG systems
- ✅ Compared 3 vector databases
- ✅ Implemented hybrid search + re-ranking
- ✅ Created production-ready web app
- ✅ Achieved 95% search accuracy
- ✅ Learned deployment patterns

**Time Invested:** ~44 hours (6-7 hours/day)

**Lines of Code:** ~1,000+ lines

**Key Takeaway:** RAG is not just retrieval - it's about combining the right techniques (embeddings + keyword + re-ranking) to get accurate, cited results

---

## Week 2: Model Context Protocol (MCP) Development 🚀 IN PROGRESS

### 🔷 [Day 8: MCP Calculator Server](https://github.com/nyalamrithwik-oss/day8-mcp-basics) ✅ COMPLETE
My first MCP server - learned how to build tools that Claude can use!

**What I Built:**
- MCP server with 5 mathematical operations
  - `add` - Add two numbers
  - `subtract` - Subtract two numbers
  - `multiply` - Multiply two numbers
  - `divide` - Divide with zero handling
  - `power` - Exponentiation
- Comprehensive test suite (5/5 passing)
- Error handling (division by zero)
- Decimal and negative number support
- Professional 5-page documentation

**Key Learnings:**
- MCP architecture (client-server model)
- Tool registration vs. execution
- Async Python patterns with asyncio
- Stdio transport protocol
- JSON Schema for input validation

**What is MCP?**
Model Context Protocol (MCP) is Anthropic's open standard for connecting AI systems like Claude to external tools and data sources. Think of it as "USB ports for AI" - a universal way to plug in tools.

**Why MCP Matters:**
- Without MCP: AI systems are isolated, can only work with static documents
- With MCP: AI systems can access live databases, APIs, tools, and real-time data

**Tech Stack:** Python 3.11, MCP SDK 1.25.0, pydantic, asyncio

**Stats:** ~200 lines of code | 4 hours | 5/5 tests passing | 100% coverage

**Documentation:** 5 pages with architecture diagrams, code examples, troubleshooting

---

### Day 9-14: Coming Soon ⏳

**Day 9:** Claude Desktop Integration + Database MCP Server
**Day 10-12:** Advanced MCP patterns + Custom tools
**Day 13-14:** Portfolio Project #2 (RAG + MCP combined)

---

## Week 3: Advanced Integration ⏳ STARTING SOON

**Focus:** Production patterns, deployment, monitoring

**Projects:**
- Day 15-17: API development and authentication
- Day 18-20: Cloud deployment (AWS/GCP)
- Day 21: Portfolio Project #3

---

## Week 4: Launch & Revenue ⏳ FINAL PUSH

**Focus:** Client acquisition, project delivery, revenue generation

**Projects:**
- Day 22-24: Client project templates
- Day 25-27: Marketing and sales
- Day 28-30: First paid projects + Final portfolio project

**Goal:** $3,000-$5,000 in signed contracts or completed work

---

## 📈 Overall Stats

| Metric | Value |
|--------|-------|
| **Days Completed** | 8/30 (26.7%) |
| **Time Invested** | ~44 hours |
| **Projects Built** | 4 complete systems |
| **Public Repositories** | 5 repos |
| **Lines of Code** | ~1,200+ lines |
| **Tests Passing** | 100% (all projects) |
| **Documentation** | Complete (READMEs + case studies) |
| **Portfolio Projects** | 1 (2 more planned) |

---

## 🎯 Learning Philosophy

### What Makes This Journey Different

**1. Build in Public 🌍**
- Every project on GitHub
- Weekly LinkedIn updates
- Transparent progress tracking

**2. Production Quality 💎**
- Professional documentation
- 100% test coverage
- Real-world use cases

**3. Portfolio-First 📂**
- Each project is showcase-ready
- Client-ready code and UI
- Comprehensive case studies

**4. Revenue-Focused 💰**
- Every skill maps to consulting services
- Real projects, not tutorials
- $3K-5K target by Day 30

---

## 🛠️ Tech Stack

### Core Technologies
- **Languages:** Python 3.10+
- **AI/LLM:** OpenAI GPT-4, Cohere
- **Frameworks:** LangChain, Streamlit, MCP SDK

### Vector Databases
- **ChromaDB** - Local vector storage
- **Pinecone** - Cloud vector database
- **Weaviate** - GraphQL vector database

### Tools & Libraries
- **Document Processing:** PyPDF2, python-docx
- **Search:** BM25, Cohere Re-rank
- **Web:** Streamlit, FastAPI
- **Testing:** pytest, unittest
- **Version Control:** Git, GitHub

---

## 📚 Key Resources

### Official Documentation
- [LangChain Docs](https://python.langchain.com/)
- [OpenAI API Docs](https://platform.openai.com/docs)
- [MCP Documentation](https://modelcontextprotocol.io/)
- [Anthropic MCP Blog](https://www.anthropic.com/news/model-context-protocol)

### Tutorials & Guides
- [LangChain RAG Tutorial](https://python.langchain.com/docs/tutorials/rag/)
- [Pinecone RAG Guide](https://www.pinecone.io/learn/retrieval-augmented-generation/)
- [Cohere Re-ranking](https://docs.cohere.com/docs/reranking)

### Learning Path
Each day includes:
- 📖 Reading (1 hour)
- 💻 Coding (4-5 hours)
- 📝 Documentation (1-2 hours)
- 🔄 Review & test (1 hour)

---

## 🎓 Skills Acquired

### Week 1 Skills ✅
- [x] RAG architecture and implementation
- [x] Vector embeddings and semantic search
- [x] Document processing (PDF, TXT, DOCX, MD)
- [x] LangChain framework
- [x] Vector database comparison
- [x] Hybrid search (BM25 + vector)
- [x] Cohere re-ranking
- [x] Streamlit web development
- [x] Production error handling
- [x] Git workflow and GitHub

### Week 2 Skills (In Progress) 🚀
- [x] MCP architecture understanding
- [x] Tool registration and execution
- [x] Async Python programming
- [x] JSON Schema validation
- [x] Stdio transport protocol
- [ ] Claude Desktop integration
- [ ] Database MCP servers
- [ ] Multi-tool workflows
- [ ] Resource management

### Week 3 Skills (Coming Soon) ⏳
- [ ] API development
- [ ] Authentication & security
- [ ] Cloud deployment
- [ ] Monitoring & logging
- [ ] Performance optimization

### Week 4 Skills (Coming Soon) ⏳
- [ ] Client communication
- [ ] Project scoping
- [ ] Pricing & proposals
- [ ] Project delivery

---

## 💼 Consulting Services (Day 30 Goal)

By the end of 30 days, I'll offer:

### 1. RAG System Development ($1,500-$2,500)
- Custom knowledge base systems
- Multi-format document support
- Hybrid search with re-ranking
- Beautiful web interface
- 1-2 week delivery

### 2. MCP Server Development ($1,000-$2,000)
- Custom tool development for Claude
- Database integrations
- API connections
- 1 week delivery

### 3. AI System Integration ($2,000-$3,000)
- RAG + MCP combined systems
- Production deployment
- Monitoring setup
- 2-3 week delivery

**Target:** 2-3 clients by Day 30 = $3,000-$5,000 revenue

---

## 📱 Connect With Me

**GitHub:** [@nyalamrithwik-oss](https://github.com/nyalamrithwik-oss)

**LinkedIn:** [Rithwik Nyalam](https://www.linkedin.com/in/rithwik-nyalam) - Follow my #BuildInPublic journey!

**Location:** Karimnagar, Telangana, India

**Status:** Available for AI consulting projects (Week 3-4)

---

## 🌟 Project Highlights

### Most Proud Of:
1. **Smart Knowledge Base** - My first production-ready AI app
2. **Day 8 MCP Server** - 5-page documentation, 100% test coverage
3. **Hybrid Search Implementation** - 95% accuracy with re-ranking

### What's Next:
1. **Day 9** - Connect MCP server to Claude Desktop (EXCITING!)
2. **Portfolio Project #2** - Combine RAG + MCP for powerful system
3. **Week 4** - Launch consulting services and land first clients

---

## 🎯 Success Metrics

### Technical Metrics
- ✅ All projects have 100% test coverage
- ✅ All code is production-ready
- ✅ Professional documentation for every project
- ✅ GitHub best practices (README, .gitignore, commits)

### Business Metrics
- 📊 Day 8/30: 26.7% complete
- 💼 LinkedIn engagement: Building in public
- 🎯 Target: $3K-5K by Day 30
- 📈 Portfolio projects: 1 complete, 2 planned

---

## 🙏 Acknowledgments

Learning from the best:
- **OpenAI** for GPT-4 and embeddings API
- **Cohere** for re-ranking API
- **Anthropic** for Claude and MCP
- **LangChain** for the amazing framework
- **Streamlit** for the beautiful UI framework
- **The AI community** for inspiration and support

---

## 📝 Daily Updates

Follow along on [LinkedIn](https://www.linkedin.com/in/rithwik-nyalam) where I share:
- Daily progress updates
- Key learnings
- Code snippets
- Challenges overcome
- Portfolio pieces

**Latest Post:** Day 8 Complete - Built my first MCP server! 🎉

---

## 🔥 Current Focus

**This Week (Week 2):** Learning Model Context Protocol (MCP) to connect Claude to external tools

**Today (Day 9):** Claude Desktop integration + Database MCP server

**This Month:** Generate $3K-5K in AI consulting revenue

---

## ⭐ Support This Journey

If you find this helpful:
- ⭐ Star this repository
- 🔗 Share with others learning AI
- 💬 Open an issue with questions
- 🤝 Connect on LinkedIn

---

## 📄 License

MIT License - Feel free to use this code for learning or commercial projects!

---

<div align="center">

**Built with ❤️ as part of my journey to master AI development**

**Day 8/30 | Week 2 | $3K-5K Revenue Goal**

*Last Updated: December 26, 2024*

</div>
[30_day_rag_learning_README.md](https://github.com/user-attachments/files/24347859/30_day_rag_learning_README.md)
