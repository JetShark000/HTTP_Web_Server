# Simple HTTP Web Server

## Overview
This is a basic HTTP web server implemented in Python using the `socket` library. It listens for incoming HTTP GET requests and serves static content, such as an `index.html` file or a `book.json` file.

## Features
- Handles **GET** requests for:
  - `/` → Serves `index.html`
  - `/book` → Serves `book.json`
- Uses **IPv4 (AF_INET) and TCP (SOCK_STREAM)**
- **Reuses the same port** after server restarts (`SO_REUSEADDR` option)
- **Handles basic HTTP methods** (Currently only `GET`)

## Installation & Usage
### Prerequisites
- Python 3.x installed on your system
- An `index.html` and `book.json` file in the same directory as `main.py`

### Running the Server
1. Clone the repository or copy the `main.py` file.
2. Navigate to the project directory.
3. Run the server with:
   ```sh
   python main.py
   ```
4. Open a web browser and navigate to:
   - `http://localhost:8080/` (To access `index.html`)
   - `http://localhost:8080/book` (To access `book.json`)

## Next Steps (To-Do List)
### Planned Improvements
- ✅ **Multi-threading**: Handle multiple clients concurrently
- ✅ **404 Response**: Return a proper 404 error if the file is not found
- ✅ **Logging**: Record client requests for debugging
- ✅ **Keep-Alive Support**: Enable persistent connections
- 🔄 **IPv6 Support**: Extend the server to handle IPv6 connections
- 🔄 **POST Request Handling**: Accept form data and API requests
- 🔄 **Dynamic Routing**: Serve different file types dynamically

## License
This project is free to use and modify. Feel free to contribute improvements!

---
### Author
Developed by Omar 

All the best! 👍

