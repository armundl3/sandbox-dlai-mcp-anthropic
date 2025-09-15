# Learning How to Use MCP

This repository is set up for exploring and learning the Model Context Protocol (MCP).

## Setup

### Prerequisites
- [uv](https://docs.astral.sh/uv/) package manager
- Python 3.11+ (uv will manage this automatically)

### Getting Started

1. **Clone and navigate to the repository**
   ```bash
   cd sandbox-dlai-mcp-anthropic
   ```

2. **Install dependencies and create virtual environment**
   ```bash
   # uv automatically creates and manages the virtual environment
   uv sync
   ```

3. **Start JupyterLab for exploration**
   ```bash
   uv run jupyter lab
   ```

4. **Run the ArXiv chatbot**
   ```bash
   uv run python arxiv_chatbot.py
   ```

### Alternative Setup (Traditional pip/venv)

If you prefer using pip and venv:

1. **Set up Python environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Repository Structure

- `pyproject.toml` - Project configuration and dependencies
- `requirements.txt` - Legacy pip requirements file
- `spec/` - Folder for building app specifications
- `arxiv_chatbot.py` - Standalone ArXiv search chatbot
- `nb/` - Jupyter notebooks
- `.env` - Environment variables (create with your API keys)

## Usage

After following the setup steps above, you can:

1. **Interactive Development**: Use JupyterLab for exploration and experimentation
2. **Command Line**: Run the chatbot directly with `uv run python arxiv_chatbot.py`
3. **Specifications**: Store your app specifications in the `spec/` folder
4. **Environment**: All dependencies are managed by uv for reproducible environments

### Environment Variables

Create a `.env` file in the project root:
```bash
ANTHROPIC_API_KEY=your_anthropic_api_key_here
```

## Development

Install development dependencies:
```bash
uv sync --group dev
```

Run formatting and linting:
```bash
uv run black .
uv run isort .
uv run mypy .
```