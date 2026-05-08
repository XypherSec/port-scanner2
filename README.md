# 🔍 Port Scanner

A lightweight Python port scanner that checks the status of the first 100 TCP ports on any target IP address — built for learning, labs, and quick recon tasks.

---

## ⚙️ How It Works

The tool iterates through **ports 1–100**, attempting a TCP connection to each one using Python's built-in `socket` library. It reports whether each port is **OPEN** or **CLOSED** based on the connection result.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.13 installed
- No external libraries required — uses the Python standard library only

### Installation

```bash
git clone https://github.com/XypherSec/port-scanner2.git
cd port-scanner2
```

### Usage

```bash
python port_checker.py
```

You will be prompted to enter a target IP address:

```
Enter IP address: 192.168.1.1
```

### Example Output

```
Port 1 closed
Port 21 closed
Port 22 is OPEN
Port 23 closed
Port 80 is OPEN
...
```

---

## 📋 Features

- Scans **TCP ports 1 through 100**
- 0.5-second timeout per port for fast results
- Simple, dependency-free implementation
- Works on any IP address reachable from your machine

---

## ⚠️ Disclaimer

This tool is intended for **educational purposes and authorized testing only**.  
Only scan systems you own or have **explicit written permission** to test.  
Unauthorized port scanning may be illegal in your jurisdiction.

---

## 🛠️ Potential Improvements

- [ ] Accept port range as a command-line argument
- [ ] Add service name resolution (e.g., port 22 → SSH)
- [ ] Multi-threading for faster scans
- [ ] Export results to a `.txt` or `.csv` file
- [ ] Add hostname resolution alongside IP input
- [ ] Banner grabbing for open ports

---

## 👤 Author

**XypherSec**  
GitHub: [@XypherSec](https://github.com/XypherSec)

---

## 📄 License

This project is open source. Feel free to fork, modify, and build on it.
