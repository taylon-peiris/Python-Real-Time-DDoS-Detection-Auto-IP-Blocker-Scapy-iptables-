🚀 Real-Time DDoS Detection & Auto IP Blocker

A lightweight cybersecurity project built in Python that monitors live network traffic and automatically blocks IP addresses that exceed a defined packet rate threshold.

This project demonstrates:

  Packet sniffing
  
  Traffic rate analysis
  
  Basic DDoS detection logic
  
  Linux firewall automation

🛠 How It Works

  The script listens to incoming IP packets using Scapy.
  
  It tracks how many packets each IP sends.
  
  Every second, it calculates the packet rate.
  
  If an IP exceeds the defined threshold (default: 40 packets/sec), it:
  
  Adds an iptables rule
  
  Blocks the IP immediately

⚙️ Requirements

Linux OS

Python 3

Root privileges

Scapy installed

Install Scapy:
  pip install scapy

▶️ How To Run

Run the script as root:
  sudo python3 ddos_detector.py

📌 Configuration

You can modify the detection sensitivity by changing:
  THRESHOLD = 40
