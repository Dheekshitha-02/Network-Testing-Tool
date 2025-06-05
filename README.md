# Network Testing Tool with GUI

This is a Python-based network testing tool with a graphical user interface (GUI) designed to execute and display the output of various network commands like `ping`, `traceroute`, `nslookup`, `ifconfig`, `nmap`, and `dig`. Unlike traditional command-line tools, this application allows users to input IP addresses, run tests, and view results directly in a clean, user-friendly UI built using Tkinter.

## Features
- 🔌 Client-server architecture using TCP sockets
- 📺 GUI display of command results (Tkinter)
- ✅ Test various network utilities:
  - Ping
  - Traceroute
  - NSLookup
  - Ifconfig / Route
  - Nmap scan
  - Dig command
- 🔧 Custom and predefined test options
- 📋 Display and select connected clients in server GUI
- 🎥 Video demos

## 🗂 Project Structure

CN_Network_Testing_Tool/

├── client.py # Client-side GUI tool

├── server.py # Server-side listener and GUI

├── ping.py # Executes ping command

├── tracefinal.py # Custom traceroute implementation

├── nslookup.py # Executes nslookup

├── ifconfig.py # Runs ifconfig

├── route.py # Runs route command

├── dig.py # Executes dig

├── nmap.py # Executes nmap

├── /screenshots/ # Output screenshots

├── /demo_videos/ # Demo walkthroughs

└── report.pdf # Project documentation/report

## 🛠 How to Run

### 1. Start the Server

```bash
python server.py
```
This will open the server-side GUI and begin listening for client connections.

### 2. Start the Client (on same or different machine)

```bash
python client.py
```
Enter the IP or use default 127.0.0.1 to connect to the server and start sending test commands.

🧪 Example Commands Supported

| Command      | Description                    |
| ------------ | ------------------------------ |
| `ping`       | Check connectivity and latency |
| `traceroute` | View route and hops            |
| `nslookup`   | DNS lookup of a domain or IP   |
| `dig`        | DNS query tool                 |
| `nmap`       | Port scanning                  |
| `route`      | Display routing tables         |
| `ifconfig`   | View network interfaces        |

📋 Requirements

- Python 2.7 (for Tkinter compatibility used in code)

- Platform-dependent network tools (e.g., ping, nmap, dig)

- Run as Administrator/root if needed (for raw sockets or traceroute)
