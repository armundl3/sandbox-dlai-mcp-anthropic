# Learning How to Use MCP

This repository is set up for exploring and learning the Model Context Protocol (MCP).

## Setup

### Prerequisites
- pyenv installed
- Python 3.11.10 (managed via pyenv)

### Getting Started

1. **Clone and navigate to the repository**
   ```bash
   cd sandbox-dlai-mcp-anthropic
   ```

2. **Set up Python environment**
   ```bash
   # Ensure you're using the correct Python version
   pyenv global 3.11.10
   
   # Create virtual environment
   python -m venv venv
   
   # Activate virtual environment
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install jupyterlab
   ```

4. **Start JupyterLab for exploration**
   ```bash
   jupyter lab
   ```

## Repository Structure

- `venv/` - Python virtual environment
- `spec/` - Folder for building app specifications
- `README.md` - This file with setup instructions

## Usage

After following the setup steps above, you can:

1. Use JupyterLab for interactive exploration and experimentation
2. Store your app specifications in the `spec/` folder
3. Develop and test MCP-related code in the activated virtual environment

The virtual environment ensures all dependencies are isolated and reproducible across different machines.