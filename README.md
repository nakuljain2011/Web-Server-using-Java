# 🧠 Web-Server-using-Java


This repository contains two implementations of a simple **Java-based TCP Web Server**:

1. **Single-Threaded Server** – handles one client connection at a time.
2. **Multi-Threaded Server** – handles multiple clients simultaneously using threads.

Each server is paired with a client that connects, sends a message, and receives a response from the server.

---

## 📁 Project Structure
Web-Server-using-Java/
|
│ ├── singlethread/
│ │ ├── Client.java
│ │ └── Server.java
│ │
│ └── multithread/
│ ├── Client.java
│ └── Server.java
│
├── README.md
└── .gitignore

---

## 🚀 How It Works

### ✅ Single-Threaded Server

- Handles **one client at a time**.
- New client connections must wait for the previous one to disconnect.
- Ideal for learning socket communication and control flow.

### ✅ Multi-Threaded Server

- Spawns a **new thread per client**.
- Can handle **many clients simultaneously**.
- Suitable for scaling up concurrent connections.

---

## 🛠️ How to Run

### 1. Compile the Java Files

# Navigate to the respective folder
cd src/singlethread        # or src/multithread

# Compile both client and server
javac Client.java
javac Server.java

---

Run the Server:

java Server

Run the Client:

java Client

💡 For multi-threaded client: it spawns 100 clients in parallel.

---

💡 Possible Enhancements

Convert to HTTP server (handle GET, POST)
Use ThreadPoolExecutor for efficient multi-threading
Add logging and metrics
Implement file serving from the server
Upgrade to Maven/Gradle project structure

---

✅ Requirements

Java 8 or higher
Command line or any IDE (e.g., IntelliJ, VS Code, Eclipse)

---

📄 License
This project is open-source and free to use under the MIT License.


