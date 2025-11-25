# 🚀 Market Intelligence Agent v2.0

An advanced AI-powered market intelligence platform that automates end-to-end market research using multi-agent workflows, real-time data integration, and interactive dashboards. Built with Streamlit, LangGraph, and cutting-edge LLMs.

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Latest-red)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## 🌟 Key Features

### 🔥 Real-Time Data Integration
- **Firecrawl.dev**: Advanced web scraping and content extraction
- **NewsData.io**: Real-time news aggregation and filtering
- **Tavily Search**: Intelligent web search capabilities
- **Enhanced Search**: Content discovery and processing

### 🤖 Multi-Agent AI Workflow
- **Reader Agent**: Data collection and processing from multiple sources
- **Analyst Agent**: Trend analysis and opportunity identification
- **Strategist Agent**: Strategic recommendations and action planning
- **Formatter Agent**: Report generation and export

### 📊 Interactive Dashboard
- **Plotly Visualizations**: Dynamic, interactive charts and graphs
- **Real-time Updates**: Live data refresh and filtering capabilities
- **Multiple Views**: Trends, opportunities, strategy, and timeline perspectives
- **Export Options**: PDF, DOCX, JSON, and Notion integration

### 🧠 AI Assistant
- **Groq-Powered**: Ultra-fast LLaMA3 inference for instant responses
- **Context-Aware**: Understands your current analysis data
- **Persistent Memory**: Conversation history and learning
- **Smart Suggestions**: Relevant prompts and actions

## 🛠️ Technology Stack

| Component | Technology |
|-----------|------------|
| **Frontend** | Streamlit + Plotly + Custom Components |
| **AI Workflow** | LangGraph + Multi-Agent Architecture |
| **LLMs** | Google Gemini 2.0 + Groq LLaMA3 |
| **Data Sources** | Firecrawl + NewsData.io + Tavily |
| **Visualization** | Plotly + Matplotlib + Seaborn |
| **Export** | ReportLab + python-docx + Notion API |
| **Database** | SQLite + FAISS Vector Store |

## 📦 Installation & Setup

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Git (optional, for cloning)

### 1. Clone Repository
```bash
git clone https://github.com/your-username/Market-Intelligence-Agent.git
cd Market-Intelligence-Agent
```

### 2. Create Virtual Environment (Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Environment Configuration
```bash
cp .env.example .env
```

Edit the `.env` file with your API keys:

```env
# Core APIs (Required)
GOOGLE_API_KEY=your_google_gemini_api_key_here
TAVILY_API_KEY=your_tavily_search_api_key_here

# Integration APIs (Required for full functionality)
FIRECRAWL_API_KEY=your_firecrawl_api_key_here
NEWSDATA_IO_KEY=your_newsdata_io_api_key_here
GROQ_API_KEY=your_groq_api_key_here

# Optional APIs
NOTION_API_KEY=your_notion_api_key_here

# Configuration
USER_AGENT=MarketIntelligenceAgent/2.0
```

### 5. API Key Setup Guide

#### 🔑 Required API Keys

**Google Gemini API**
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Copy to your `.env` file

**Tavily Search API**
1. Visit [Tavily](https://tavily.com)
2. Sign up for an account
3. Get your API key
4. Copy to your `.env` file

#### 🔧 Integration API Keys (Recommended)

**Firecrawl API**
1. Visit [Firecrawl.dev](https://firecrawl.dev)
2. Sign up for an account
3. Get your API key from the dashboard
4. Copy to your `.env` file

**NewsData.io API**
1. Visit [NewsData.io](https://newsdata.io)
2. Create an account
3. Get your API key
4. Copy to your `.env` file

**Groq API**
1. Visit [Groq](https://groq.com)
2. Sign up for an account
3. Get your API key
4. Copy to your `.env` file

## 🚀 Running the Application

```bash
streamlit run app.py
```

The application will open at `http://localhost:8501`

## 🎯 Feature Walkthrough

### 🏠 Home Tab - Multi-Agent Analysis
- **Enhanced Input**: Query, market domain, and specific questions
- **Advanced Options**: Data source selection and analysis depth
- **Real-time Progress**: Live agent status and workflow tracking
- **Quick Actions**: Direct navigation to results

### 📊 Dashboard Tab - Interactive Analytics
- **Dynamic Charts**: Plotly-powered interactive visualizations
- **Filtering**: Real-time data filtering and exploration
- **Multiple Views**: Trends, opportunities, strategy, and timeline
- **Export Options**: Chart and data export functionality

### 📄 Report Tab - Comprehensive Analysis
- **Structured Reports**: AI-generated markdown reports
- **Multiple Formats**: PDF, DOCX, and Notion export
- **Chart Integration**: Embedded visualizations
- **Download Options**: Complete analysis packages

### 🤖 Assistant Tab - AI-Powered Chat
- **Context-Aware**: Understands your current analysis
- **Fast Responses**: Groq-powered instant inference
- **Smart Suggestions**: Pre-built prompts and actions
- **Persistent Memory**: Conversation history and learning

### 📚 History Tab - Analysis Management
- **Session Management**: Load and manage previous analyses
- **Bulk Operations**: Export and delete multiple analyses
- **Search & Filter**: Find specific analyses quickly
- **Analytics**: Usage statistics and insights

## 🔧 Architecture Overview

### Multi-Agent Workflow
```
Input → Reader Agent → Analyst Agent → Strategist Agent → Formatter Agent → Output
         ↓              ↓               ↓                  ↓
    Data Collection  Analysis      Strategy Planning   Report Generation
    - Web Scraping   - Trends      - Recommendations   - Charts
    - News APIs      - Opportunities - Action Plans    - Exports
    - Content Filter - Competitive  - Risk Assessment  - Dashboards
```

### Data Flow
1. **Collection**: Reader Agent gathers data from multiple sources
2. **Analysis**: Analyst Agent processes data and extracts insights
3. **Strategy**: Strategist Agent generates recommendations and plans
4. **Formatting**: Formatter Agent creates reports and visualizations
5. **Interaction**: Assistant provides ongoing support and Q&A

## 🔍 Usage Examples

### Basic Market Analysis
1. Enter query: "AI trends in healthcare"
2. Select domain: "Healthcare"
3. Click "Run Multi-Agent Analysis"
4. Explore results in Dashboard and Report tabs

### Advanced Analysis with Assistant
1. Complete basic analysis
2. Go to Assistant tab
3. Ask: "What are the key risks in my analysis?"
4. Follow up: "How can I validate these opportunities?"

### Export and Sharing
1. Navigate to Report tab
2. Choose export format (PDF/DOCX)
3. Download comprehensive report
4. Share with stakeholders

## 🚀 Advanced Features

### Custom Agent Configuration
- Modify agent behavior in `core/agents/`
- Adjust analysis depth and focus areas
- Configure data source priorities

### Integration Extensions
- Add new data sources in `core/integrations/`
- Implement custom export formats
- Extend chart generation capabilities

### Dashboard Customization
- Modify visualizations in `components/ui_dashboard.py`
- Add new chart types and filters
- Customize metrics and KPIs

## 🔧 Troubleshooting

### Common Issues

**API Key Errors**
- Verify all required API keys are set in `.env`
- Check API key validity and quotas
- Ensure proper formatting (no extra spaces)

**Import Errors**
- Run `pip install -r requirements.txt`
- Check Python version compatibility (3.8+)
- Verify virtual environment activation

**Performance Issues**
- Reduce analysis depth for faster results
- Limit data sources for quicker processing
- Check internet connection for API calls

**Chart Generation Failures**
- Ensure sufficient data for visualization
- Check Plotly and Matplotlib installations
- Verify output directory permissions

### Debug Mode
Enable debug logging by setting in `.env`:
```env
LOG_LEVEL=DEBUG
```

## 📁 Project Structure
```
Market-Intelligence-Agent/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── .env.example          # Environment variable template
├── LICENSE               # MIT License
├── components/           # UI components for each tab
│   ├── ui_home.py        # Home tab UI
│   ├── ui_dashboard.py   # Dashboard tab UI
│   ├── ui_report.py      # Report tab UI
│   ├── ui_assistant.py   # Assistant tab UI
│   └── ui_history.py     # History tab UI
├── config/               # Configuration files
│   └── settings.py       # Application settings
├── core/                 # Core application logic
│   ├── agents/           # Multi-agent implementations
│   │   ├── reader_agent.py
│   │   ├── analyst_agent.py
│   │   ├── strategist_agent.py
│   │   └── formatter_agent.py
│   ├── integrations/     # API clients
│   │   ├── firecrawl_client.py
│   │   ├── groq_client.py
│   │   └── newsdata_client.py
│   ├── workflow/         # Agent orchestration
│   │   └── agent_orchestrator.py
│   ├── charts/           # Chart generation
│   ├── export/           # Export functionality
│   └── utils.py          # Utility functions
├── reports/              # Generated reports (created at runtime)
├── assets/               # Static assets (created at runtime)
└── exports/              # Exported files (created at runtime)
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google Gemini** for advanced language understanding
- **Groq** for fast inference capabilities
- **Firecrawl** for intelligent web scraping
- **NewsData.io** for real-time news aggregation
- **Streamlit** for the amazing web framework
- **Plotly** for interactive visualizations
- **LangChain/LangGraph** for AI workflow orchestration

## 📞 Support

For support, questions, or feature requests:
- Create an issue on GitHub
- Check the troubleshooting section
- Review the documentation

---

**🚀 Market Intelligence Agent v2.0** - Transforming market research with AI-powered multi-agent workflows.