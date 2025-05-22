# Hochiri – Personality Chatbot

Hochiri is a desktop chatbot with a strong, blunt personality, built with Python, OpenRouter (OpenAI-compatible API), and a modern Tkinter GUI (ttkbootstrap).  
The bot keeps short- and long-term memory, can summarize conversations, and is designed to be concise, sarcastic, and not overly friendly.

---

## Features

- **Personality:** Hochiri is confident, sometimes rude, never overly nice, and always concise.
- **GUI:** Modern, dark-themed chat window using [ttkbootstrap](https://ttkbootstrap.readthedocs.io/).
- **Memory:** Keeps short-term and long-term (summarized) conversation memory.
- **Summarization:** Automatically summarizes conversations after a set number of prompts.
- **Logging:** All conversations are logged to `logs/session.log` and `logs/history.log`.

---

## Requirements

- Python 3.9+
- [openai](https://pypi.org/project/openai/)
- [ttkbootstrap](https://pypi.org/project/ttkbootstrap/)

Install dependencies:
```bash
pip install openai ttkbootstrap
```

---

## Setup

1. **Clone the repository:**
    ```bash
    git clone https://github.com/BrawlsMons/OpenRouter-Ai-Assistante.git
    cd OpenRouter-Ai-Assistante
    ```

2. **Insert your OpenRouter API key:**
    - Open `main.py`
    - Replace `[YOUR_API_KEY]` with your actual OpenRouter API key:
      ```python
      API_KEY = "sk-..."  # Your OpenRouter API key here
      ```

3. **Run the bot:**
    ```bash
    python main.py
    ```

---

## Usage

- Type your message and press **Enter** or click **Send**.
- After every 5 prompts, Hochiri will automatically summarize the conversation.
- You can also click **Summarize** to force a summary at any time.

---

## File Structure

- `main.py` – Main application code (GUI, logic, memory, logging)
- `logs/` – Session and history logs (created automatically)
- `.gitignore` – Should include `logs/`, `.venv/`, and other temp files

---

## License

MIT License

Copyright (c) 2025 BrawlsMons

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

## Credits

- [OpenRouter](https://openrouter.ai/) for API access
- [ttkbootstrap](https://ttkbootstrap.readthedocs.io/) for modern Tkinter themes

---

**Note:**  
Do **not** commit your real API keys to public repositories!
