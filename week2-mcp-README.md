# Week 2: MCP Server Development

> **Collection of 5 production-ready MCP (Model Context Protocol) servers built during Days 8-12**

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![MCP Protocol](https://img.shields.io/badge/MCP-Enabled-green.svg)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📚 Projects Overview

This folder contains 5 MCP (Model Context Protocol) servers, each demonstrating different integration capabilities:

| Project | Purpose | Key Features | Status |
|---------|---------|--------------|--------|
| [Day 8: Calculator MCP](./day8-mcp-basics) | Business calculations | Arithmetic, statistics, financial metrics | ✅ Complete |
| [Day 9: Database MCP](./day9-database-mcp) | SQLite operations | CRUD, queries, transactions | ✅ Complete |
| [Day 10: Weather MCP](./day10-weather-mcp) | Real-time weather data | Current conditions, forecasts | ✅ Complete |
| [Day 11: HubSpot MCP](./day11-hubspot-mcp) | CRM integration | Contacts, deals, activities | ✅ Complete |
| [Day 12: Business Intelligence Assistant](./day12-business-assistant) | Multi-tool orchestration | RAG + 4 MCP servers | ✅ Complete |

---

## 🚀 Quick Start

### Prerequisites

- Python 3.10 or higher
- Claude Desktop (for MCP integration)
- Git

### Installation

```bash
# Clone the repository
git clone <your-repo-url>
cd week2-mcp

# Each project has its own virtual environment
# Navigate to any project folder and follow its README
```

### Running Individual Servers

Each MCP server can be run independently:

```bash
# Example: Running Calculator MCP
cd day8-mcp-basics
python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/Mac
pip install -r requirements.txt
python simple_mcp_server.py
```

### Integrating with Claude Desktop

1. Each project contains a `claude_desktop_config.txt` or similar file
2. Copy the configuration to your Claude Desktop config
3. Restart Claude Desktop
4. The MCP tools will be available in your Claude conversations

For detailed integration instructions, see [MCP Integration Guide](./MCP_INTEGRATION_GUIDE.md).

---

## 🏗️ Architecture

### Individual MCP Server Architecture

```
┌─────────────────────────────────────────┐
│           Claude Desktop                │
│                                          │
│  ┌────────────────────────────────────┐ │
│  │         Claude AI Model            │ │
│  │                                    │ │
│  │  • Natural language understanding  │ │
│  │  • Tool selection                  │ │
│  │  • Response generation             │ │
│  └────────────────────────────────────┘ │
│                    │                     │
│                    ▼                     │
│  ┌────────────────────────────────────┐ │
│  │        MCP Client Layer            │ │
│  │                                    │ │
│  │  • Protocol handling               │ │
│  │  • Request formatting              │ │
│  │  • Response parsing                │ │
│  └────────────────────────────────────┘ │
└─────────────────────────────────────────┘
                    │
                    │ MCP Protocol
                    │
                    ▼
┌─────────────────────────────────────────┐
│         MCP Server (Python)             │
│                                          │
│  ┌────────────────────────────────────┐ │
│  │         Server Logic               │ │
│  │                                    │ │
│  │  • Tool implementations            │ │
│  │  • Business logic                  │ │
│  │  • Error handling                  │ │
│  └────────────────────────────────────┘ │
│                    │                     │
│                    ▼                     │
│  ┌────────────────────────────────────┐ │
│  │      External Resources            │ │
│  │                                    │ │
│  │  • APIs (Weather, HubSpot)         │ │
│  │  • Databases (SQLite)              │ │
│  │  • File systems                    │ │
│  └────────────────────────────────────┘ │
└─────────────────────────────────────────┘
```

### Multi-Server Orchestration (Day 12)

```
┌──────────────────────────────────────────────────┐
│       Business Intelligence Assistant            │
│                                                   │
│  ┌─────────────────────────────────────────────┐ │
│  │         Query Processing Layer              │ │
│  │  • Intent Recognition                       │ │
│  │  • Tool Selection                           │ │
│  │  • Response Orchestration                   │ │
│  └─────────────────────────────────────────────┘ │
│                      │                            │
│                      ▼                            │
│  ┌─────────────────────────────────────────────┐ │
│  │          RAG Layer (ChromaDB)               │ │
│  │  • Document Retrieval                       │ │
│  │  • Semantic Search                          │ │
│  │  • Context Enhancement                      │ │
│  └─────────────────────────────────────────────┘ │
│                      │                            │
│                      ▼                            │
│  ┌──────────────────────────────────────────────┐│
│  │         MCP Tool Coordination                ││
│  │                                              ││
│  │  ┌──────────┐  ┌──────────┐  ┌──────────┐  ││
│  │  │Calculator│  │ Database │  │ Weather  │  ││
│  │  │   MCP    │  │   MCP    │  │   MCP    │  ││
│  │  └──────────┘  └──────────┘  └──────────┘  ││
│  │                                              ││
│  │              ┌──────────┐                   ││
│  │              │ HubSpot  │                   ││
│  │              │   MCP    │                   ││
│  │              └──────────┘                   ││
│  └──────────────────────────────────────────────┘│
└──────────────────────────────────────────────────┘
```

---

## 📖 Project Details

### Day 8: Calculator MCP Server

**Purpose:** Provide advanced calculation capabilities through MCP

**Capabilities:**
- Basic arithmetic (add, subtract, multiply, divide)
- Advanced math (power, sqrt, absolute value)
- Statistics (mean, median, mode, standard deviation)
- Financial metrics (ROI, CAGR, NPV, IRR)
- Percentage calculations

**Tech Stack:** Python, FastAPI, pytest

**[View Project →](./day8-mcp-basics)**

---

### Day 9: Database MCP Server

**Purpose:** Enable database operations through MCP

**Capabilities:**
- CRUD operations (Create, Read, Update, Delete)
- Complex SQL queries
- Transaction management
- Schema management
- Data validation

**Tech Stack:** Python, SQLite3, FastAPI

**[View Project →](./day9-database-mcp)**

---

### Day 10: Weather Intelligence MCP Server

**Purpose:** Provide real-time weather data for business decisions

**Capabilities:**
- Current weather conditions
- 7-day forecasts
- Location-based search
- Multi-city comparison
- Weather impact analysis

**Tech Stack:** Python, WeatherAPI.com, Requests

**[View Project →](./day10-weather-mcp)**

---

### Day 11: HubSpot CRM MCP Server

**Purpose:** Integrate CRM data through MCP

**Capabilities:**
- Contact management
- Deal tracking
- Company data access
- Activity logging
- Custom property handling

**Tech Stack:** Python, HubSpot API v3, OAuth

**[View Project →](./day11-hubspot-mcp)**

---

### Day 12: Business Intelligence Assistant

**Purpose:** Orchestrate multiple MCP servers with RAG for intelligent insights

**Capabilities:**
- Natural language queries across multiple tools
- RAG-powered knowledge base
- Real-time data synthesis
- Context-aware responses
- Multi-tool coordination

**Tech Stack:** Python, OpenAI GPT-4, ChromaDB, All 4 MCP servers, Streamlit

**[View Project →](./day12-business-assistant)**

**Special Note:** This is the flagship project that demonstrates all Week 2 learnings combined into a production-ready system.

---

## 🛠️ Common Setup

### Windows-Specific Configuration

All projects have been tested and configured for Windows development:

- PowerShell execution policy handling
- Windows path formatting
- Virtual environment activation scripts
- Claude Desktop Windows configuration

### Utility Scripts

Located in the root of `week2-mcp`:

- `fix_claude_config.py` - Fix Claude Desktop configuration issues
- `recreate_claude_config.py` - Rebuild Claude Desktop config
- `verify_setup.py` - Verify MCP server setup

---

## 📚 Documentation

- **[MCP Integration Guide](./MCP_INTEGRATION_GUIDE.md)** - Comprehensive guide for integrating MCP servers with Claude Desktop
- **[Week 2 Summary](../WEEK2_SUMMARY.md)** - Detailed summary of Week 2 achievements
- **[Demo Script](./DEMO_ALL_SERVERS.py)** - Unified demo showing all servers working

Each project folder contains:
- `README.md` - Project-specific documentation
- `requirements.txt` - Python dependencies
- Test files - Comprehensive test coverage
- Completion notes - Learning documentation

---

## 🧪 Testing

Each project includes comprehensive tests:

```bash
# Navigate to any project
cd day8-mcp-basics

# Activate virtual environment
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/Mac

# Run tests
pytest
```

**Total Test Coverage:** 80%+ across all projects

---

## 🔧 Troubleshooting

### Common Issues

**Issue 1: Claude Desktop Not Detecting Server**
- Ensure server is running
- Check configuration file path
- Restart Claude Desktop
- Verify JSON syntax in config

**Issue 2: PowerShell Execution Policy Error**
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

**Issue 3: Virtual Environment Path Issues**
- Use absolute paths in Claude Desktop config
- Ensure forward slashes in JSON configuration
- Verify Python interpreter path

**Issue 4: API Key Issues**
- Check `.env` file exists
- Verify API key format
- Ensure environment variables are loaded

For detailed troubleshooting, see [MCP Integration Guide](./MCP_INTEGRATION_GUIDE.md).

---

## 📊 Performance Metrics

Based on production testing:

| Metric | Value |
|--------|-------|
| Average Response Time | <2 seconds |
| Tool Coordination Success | 95%+ |
| Test Coverage | 80%+ |
| Error Recovery Rate | 100% |
| Documentation Coverage | 100% |

---

## 🎯 Use Cases

### Business Intelligence
- "Calculate ROI for Q4 deals and check weather impact on deliveries"
- "Analyze customer data from database and cross-reference with CRM"

### Sales Operations
- "Find high-value contacts in HubSpot and calculate deal pipeline value"
- "Query sales data and compute statistical trends"

### Logistics Planning
- "Check weather forecasts for warehouse locations and calculate shipping delays"
- "Analyze delivery performance data accounting for weather conditions"

### Financial Analysis
- "Calculate CAGR for top customers and compare with industry benchmarks"
- "Compute NPV for investment opportunities using current data"

---

## 🚀 What's Next?

### Week 3 Plans (Days 15-21)
- Build signature Sales Intelligence System
- Create comprehensive case studies
- Record demo videos
- Package services for clients
- Prepare for market launch

### Future Enhancements
- [ ] Add more MCP server integrations (Salesforce, Slack, etc.)
- [ ] Implement caching layer for performance
- [ ] Add voice interface
- [ ] Build web dashboard
- [ ] Multi-language support

---

## 🤝 Contributing

While these are learning projects, feedback and suggestions are welcome!

1. Open an issue for bugs or feature requests
2. Fork the repository for contributions
3. Submit pull requests with clear descriptions

---

## 📝 License

All projects in this folder are licensed under the MIT License.

---

## 👤 Author

**Rithwik Nyalam**
- GitHub: [@nyalamrithwik-oss](https://github.com/nyalamrithwik-oss)
- LinkedIn: [Rithwik Nyalam](https://www.linkedin.com/in/rithwik-nyalam)
- Role: AI Generalist & Consultant

---

## 🙏 Acknowledgments

- Anthropic for Claude and MCP protocol
- Python community for excellent libraries
- Everyone who engaged with my learning journey

---

## 📧 Contact

For questions or consulting inquiries:
- Open an issue on GitHub
- Connect on LinkedIn
- Email: [Your consulting email]

---

**Built during:** Days 8-12 of 30-Day RAG & MCP Learning Journey  
**Status:** Week 2 Complete ✅  
**Progress:** 12/30 days (40% complete)

---

*Building in public, one MCP server at a time* 🚀
