# Network Quiz Game (c203)

A multi-threaded TCP quiz game where the server sends random trivia questions and clients answer via a Tkinter chat-style GUI.

## Features
- TCP server (port 8000) accepting multiple concurrent clients, each on its own thread
- Random trivia question bank (science, geography, general knowledge) with multiple-choice answers
- Score tracking per client
- Tkinter GUI client with login screen, chat-style question/answer layout, and scrollback

## Tech Stack
- Python 3 (standard library only)
- `socket`, `threading`, `random`
- `tkinter` for the GUI client

## Project Structure
```
c203/
├── server.py     # quiz server
└── client.py     # Tkinter GUI client
```

## Installation
No third-party dependencies (uses the Python standard library). Requires a Python build with Tkinter support.

## Usage
Start the server first:
```bash
python server.py
```
Then run one or more clients (in separate terminals):
```bash
python client.py
```
Enter a name, answer each question with `a`, `b`, `c`, or `d`, and track your score.