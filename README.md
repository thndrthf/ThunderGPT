
# ThunderGPT v4

A simple offline desktop chat app for Ollama, built with Python and Tkinter.

This app talks only to your local Ollama server at `http://127.0.0.1:11434` and gives you a lightweight GUI for chatting with local models without needing a browser or cloud service.


<img width="855" height="553" alt="Screenshot 2026-04-07 at 9 08 44 AM" src="https://github.com/user-attachments/assets/b0b5a809-0b50-4340-903a-24ba31cea89e" />

## Features

- Fully local/offline Ollama frontend
- Tkinter desktop GUI
- Auto-checks whether Ollama is running
- Attempts to start `ollama serve` automatically
- Lists locally installed Ollama models
- Editable system prompt
- Streaming assistant replies
- Stop button for interrupting generation
- Adjustable temperature
- Adjustable max token output
- New chat button
- Save transcript as Markdown

## How it works

The app connects to these local Ollama endpoints:

- `/api/tags` for model listing and health checks
- `/api/chat` for streaming chat responses

It does not depend on any remote API and is designed for local-first use.

## Requirements

- Python 3.x
- Ollama installed
- At least one local Ollama model pulled
- Python packages:
  - `requests`
  - `tkinter` (usually included with Python)

## Install

Install Python dependency:

```bash
pip install requests
