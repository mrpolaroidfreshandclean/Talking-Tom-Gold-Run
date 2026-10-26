# 🎮 Welcome to the Talking Tom Gold Run Tutorial!

<img width="720" height="352" alt="Talking Tom Gold Run" src="https://github.com/user-attachments/assets/d9a9e2ac-25c3-4a87-98d6-0641ff0baef4" />

This tutorial will teach you how to run **Talking Tom Gold Run** locally using a simple Python HTTP server.

## ⚠️ Requirements

You will need to install **Python** because the game requires a local web server to run.

**Download Python here:** https://www.python.org/

## 📁 Step 1 — Locate the Game Files

First, navigate to the folder containing the Talking Tom Gold Run game files.

<img width="612" height="377" alt="Game Files" src="https://github.com/user-attachments/assets/5297349f-7d44-48a3-9340-ab02017bd1b4" />

Make sure you are inside the correct directory before continuing.

---

## ⚙️ Step 2 — Create the Start Script

Inside the game folder, create a new file named `start.bat`.

Open it with a text editor, such as Notepad, and paste the following code:

```bat
@echo off
python -c "import mimetypes; from http.server import SimpleHTTPRequestHandler, ThreadingHTTPServer; mimetypes.add_type('text/javascript', '.mjs'); ThreadingHTTPServer(('127.0.0.1', 8111), SimpleHTTPRequestHandler).serve_forever()"
pause
```

You can download the script directly from the project repository:

**[Download start.bat](https://github.com/mrpolaroidfreshandclean/Talking-Tom-Gold-Run/blob/main/start.ba)**
You can also inspect the code before running it.

Save the file and make sure its name is `start.bat`, not `start.bat.txt`.


### 🔌 Choosing a Port

IF YOU DECIDE TO CHANGE
THE PORT AFTER YOU PLAYED 
YOUR GAME DATA WILL BE GONE
*i will make a guide how to change the port without losing the game data*

Look at this part of the .bat code:

```python
ThreadingHTTPServer(('127.0.0.1', 8111), SimpleHTTPRequestHandler)
```

The number `8111` is the **port** used by the local server.

If port `8111` is already in use, you can try another port, such as:

- `8080`
- `3000`
- `8000`
- `5500`

For example, to use port `8080`, change the code to:

```python
ThreadingHTTPServer(('127.0.0.1', 8080), SimpleHTTPRequestHandler)
```

**Important:** Remember which port you selected. You will need it in the next step.

### ▶️ Start the Server

Double-click `start.bat` to launch the local server.

A Command Prompt window will open. Keep this window open while playing the game.

<img width="989" height="517" alt="Local Server Running" src="https://github.com/user-attachments/assets/7ea4e177-b7ee-4064-8902-fa81b96b08d7" />

## 🌐 Step 3 — Open the Game in Your Browser

Now open your web browser and enter the following address:

```text
http://localhost:SERVERPORT
```

**For example:**
- Port `8111` → `http://localhost:8111`
- Port `8080` → `http://localhost:8080`
- Port `5500` → `http://localhost:5500`

Press **Enter**, and the game should load in your browser!

<img width="950" height="768" alt="Talking Tom Gold Run Running Locally" src="https://github.com/user-attachments/assets/35fe9907-adee-4793-8cf3-fdec90f8c795" />

---

## 🎉 That's It!

*Any problems? go here https://github.com/mrpolaroidfreshandclean/Talking-Tom-Gold-Run/issues*

### ❤️ Credits

All credits go to **[@Task4z](https://github.com/Task4z)** and **[@xdijd](https://github.com/xdijd)** for their work on this project.

This tutorial documents a way to run the game locally using Python.

**Enjoy playing Talking Tom Gold Run!** 🎮
