# CodeAlpha Basic Network Sniffer

## Project Overview
This project was completed as part of the CodeAlpha Cyber Security Internship.

The objective of this project is to capture and analyze network traffic packets using Python and the Scapy library.

---

## Features
- Captures live network packets
- Displays packet summaries
- Demonstrates basic packet sniffing
- Helps understand network communication

---

## Technologies Used
- Python
- Scapy
- VS Code

---

## Installation

### Install Python
Download Python from:
https://www.python.org/downloads/

### Install Scapy
Run the following command:

```bash
pip install scapy
```

---

## Python Code

```python
from scapy.all import sniff

# Function to process packets
def packet_callback(packet):
    print(packet.summary())

print("Starting Network Sniffer...")

# Capture 20 packets
sniff(prn=packet_callback, count=20)
```

---

## How to Run

Open terminal and run:

```bash
python sniffer.py
```

---

## Expected Output

```bash
Starting Network Sniffer...
Ether / IP / TCP 192.168.1.5 > 142.250.190.78
Ether / IP / UDP 8.8.8.8 > 192.168.1.5
```

---

## Learning Outcome
This project helped in understanding:

- Packet sniffing
- Network protocols
- Traffic analysis
- Cybersecurity monitoring
- Python networking libraries

---

## Files Included
- sniffer.py
- README.md
- Screenshots

---

## Author
Kareem Folashade Kafayat 
