# AI-weather-mcp-server
MCP Server
There’s a list of public MCP servers here:

👉 https://github.com/modelcontextprotocol/servers

👉 Weather MCP Server — https://github.com/mschneider82/mcp-openweather


<img width="853" height="430" alt="image" src="https://github.com/user-attachments/assets/6012f4d0-75a7-4786-ba70-f67498d3c64a" />
<img width="758" height="411" alt="image" src="https://github.com/user-attachments/assets/c92e7669-5dd9-441f-a1f6-4961b13e7dda" />


Environment setup:
Setting Up the Weather MCP Server:
Step 1 – Install Go: https://go.dev/dl/

Step 2 - Clone and Build

	git clone https://github.com/mschneider82/mcp-openweather.git

	cd mcp-openweather
	
	go build -o mcp-weather

Step 3 – Get OpenWeatherMap API Key
	1.	Visit https://openweathermap.org/api
	2.	Create a free account.
	3.	Copy your API key (called appid).
	4.	If it doesn’t work right away — wait a few hours.
Run the MCP Server Locally:
./mcp-weather  (⚠️ Keep this terminal running, this is your MCP server.)


pip install python-dotenv langchain-mcp-adapters langgraph "langchain[openai]" mcp 
Adding a Second MCP Server – Calculator
Install:

	pip install mcp-server-calculator
	
Run in separate terminals:

	Terminal 1 — Weather MCP Server
	
		.\mcp-weather.exe

	Terminal 2 — Calculator MCP Server
	
		python -m mcp_server_calculator

	Terminal 3 — Your Client
	
		python 1.py
