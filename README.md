# ACPXMCP - AI Agent Communication Platform

A powerful AI agent communication platform that integrates multiple AI frameworks for enhanced agent interactions and task execution.

## 🚀 Tech Stack

- **Python 3.8+** - Core programming language
- **CrewAI** - Multi-agent orchestration framework
- **SmoLAgents** - Lightweight agent framework
- **MCP (Model Context Protocol)** - Agent communication protocol
- **FastAPI/Flask** - Web server framework (inferred from server files)
- **Additional dependencies** - As specified in requirements.txt

## 📋 Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- Git

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/MOHAMMADIBRAHIMKHAN/ACPXMCP.git
cd ACPXMCP
```

### 2. Install Dependencies

Install all required packages from requirements.txt:

```bash
pip install -r requirements.txt
```

### 3. Environment Configuration

Create a `.env` file in the root directory and add your configuration variables:

```bash
# Example .env file
API_KEY=your_api_key_here
DATABASE_URL=your_database_url
# Add other environment variables as needed
```

**Note:** The `.env` file is ignored by Git for security purposes.

## 🏃‍♂️ How to Run

### Step 1: Start the SmoLAgents Server

First, run the SmoLAgents server to initialize the lightweight agent framework:

```bash
python smolagents_server.py
```

This will start the SmoLAgents server and prepare the agent communication infrastructure.

### Step 2: Start the Crew Agent Server (Optional)

If you need CrewAI functionality, run the crew agent server in a separate terminal:

```bash
python crew_agent_server.py
```

### Step 3: Execute Main Application

Finally, run the main application to get your results:

```bash
python runACPXMCP.py
```

This script will:
- Initialize the ACPXMCP platform
- Connect to the running agent servers
- Process your queries and return results

## 📁 File Structure

```
ACPXMCP/
├── crew_agent_server.py    # CrewAI agent server implementation
├── smolagents_server.py    # SmoLAgents server implementation  
├── runACPXMCP.py          # Main execution script
├── requirements.txt        # Python dependencies
├── .env                   # Environment variables (not tracked)
├── .gitignore            # Git ignore rules
└── README.md             # This file
```

## 🔧 Usage

1. **Start Servers**: Begin by running `smolagents_server.py` to initialize the agent infrastructure
2. **Optional CrewAI**: If using CrewAI features, also run `crew_agent_server.py`
3. **Execute Main**: Run `runACPXMCP.py` to start processing and get your answers
4. **Monitor Output**: Check the console output for results and any error messages

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 Notes

- Ensure all servers are running before executing the main script
- Check the console output for any error messages or debugging information
- Make sure your `.env` file contains all necessary configuration variables
- For production deployment, consider using process managers like PM2 or systemd

## 🐛 Troubleshooting

- **Import Errors**: Make sure all dependencies are installed via `pip install -r requirements.txt`
- **Server Connection Issues**: Ensure servers are running and ports are not blocked
- **Environment Variables**: Verify your `.env` file contains all required variables
- **Python Version**: Confirm you're using Python 3.8 or higher

## 📧 Contact

For questions or support, please open an issue on this repository.

---

**Built with ❤️ using Python and AI Agent Frameworks**