# Python ICMP Ping Implementation

This repository demonstrates a **low-level ICMP Ping utility** written in Python.  
It showcases how raw sockets work by manually constructing and sending **ICMP Echo Requests**, then parsing and validating **ICMP Echo Replies**.

The project include:
- A **python code** (`.py`) containing the complete implementation and live execution flow.

---

## Repository Structure

project-root/

├─ icmp_ping.py # Jupyter Notebook with full ICMP Ping implementation

markdown
Copy code

---

## Features

- 🌐 **ICMP Echo Requests/Replies** – send pings and capture replies using raw sockets.  
- ⚙️ **Manual Packet Construction** – checksum calculation, header encoding, and payload definition.  
- 🕒 **Timeout & Latency Measurement** – measure round-trip times with configurable timeout.  
- 📡 **Cross-Platform (with Admin Rights)** – works on systems that allow raw socket creation.  
- 📑 **Report Included** – PDF with explanation, methodology, and sample outputs.  

---

## Requirements

- Python **3.8+**
- Jupyter Notebook or JupyterLab (for interactive use)
- Administrative / root privileges (required for raw socket creation)

**Dependencies (standard library only):**
- `socket`
- `struct`
- `time`
- `select`
- `binascii`
- `os`
- `sys`

---

## Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/python-icmp-ping.git
   cd python-icmp-ping
Run the notebook interactively:

bash
Copy code
jupyter notebook
Or convert and run as a script:

bash
Copy code
jupyter nbconvert --to script Python_Ping.ipynb
sudo python Python_Ping.py   # requires sudo for raw sockets
How It Works
- Constructs ICMP Echo packets with headers and checksum.
- Sends packets to a specified destination host.
- Listens for replies on a raw socket with timeout control.
- Calculates latency and displays results similar to the system ping utility.

This implementation provides an educational view into network protocols at the transport layer and demonstrates how Python can interact directly with the Internet Control Message Protocol (ICMP).
