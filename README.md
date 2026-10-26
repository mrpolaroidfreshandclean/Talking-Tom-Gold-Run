# Talking Tom Gold Run - HTML Port

> **Credits:** Port developed by **@Task4z** and **@xdijd**.

<img width="720" height="352" alt="Banner" src="https://github.com/user-attachments/assets/d9a9e2ac-25c3-4a87-98d6-0641ff0baef4" />

---

## ⚠️ Requirements
<span style="color: red;">**You will need to download Python!**</span> (Because you need to run a local server to play).  
🔗 [Download Python here](https://www.python.org/)

---

## 🚀 How to Run the Game

### Step 1: Open the Game Files
Go to the folder where your game files are located.

<img width="612" height="377" alt="Game Files" src="https://github.com/user-attachments/assets/5297349f-7d44-48a3-9340-ab02017bd1b4" />

---

### Step 2: Create a Start Script (`.bat`)
Create a new text file inside the folder, paste the code below, and save it as **`start.bat`**:

```python
python -c "import mimetypes; from http.server import SimpleHTTPRequestHandler, ThreadingHTTPServer; mimetypes.add_type('text/javascript', '.mjs'); ThreadingHTTPServer(('127.0.0.1', 8111), SimpleHTTPRequestHandler).serve_forever()"
