# PaperPal 📚

An Intelligent Academic Research Companion

## Overview

PaperPal is an AI-powered research assistant that helps researchers and students efficiently process, analyze, and understand academic papers. It combines state-of-the-art language models with intelligent agents to provide features like paper summarization, concept extraction, and research insights.

## Technology Stack

### Core Framework
* Frontend: Streamlit (rapid prototyping, ML-friendly)
* Agent Framework: CrewAI (multi-agent orchestration)
* Language: Python 3.9+
* Containerization: Docker + Docker Compose

### AI/ML Stack
* LLM: Ollama (Llama 3.1 8B) - local deployment
* Embeddings: sentence-transformers (all-MiniLM-L6-v2)
* NLP: spaCy (entity extraction)
* ML: transformers, scikit-learn

### Data Storage
* Vector Database: ChromaDB (document embeddings)
* Graph Database: NetworkX (concept relationships)
* File Storage: Local filesystem → Cloud storage
* Metadata: SQLite → PostgreSQL

### Visualization
* Interactive Charts: Plotly
* Network Graphs: Pyvis, streamlit-agraph
* Analytics: matplotlib, wordcloud

## Setup

1. Create a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your configuration
```

4. Run the application:
```bash
streamlit run main.py
```

## Project Structure

```
.
├── config/             # Configuration files
├── agents/             # AI agent definitions
├── services/           # Core services (PDF, Vector, LLM)
├── utils/             # Utility functions
├── ui/                # Streamlit UI components
│   ├── pages/        # Additional pages
│   └── components/   # Reusable components
├── data/             # Data storage
├── docs/             # Documentation
└── tests/            # Test files
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

