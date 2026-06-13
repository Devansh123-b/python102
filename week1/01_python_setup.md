# 01 – Setting Up Python on Your Machine

## What's different from Python101?

In Python101, you wrote code in a browser. A server somewhere ran it for you.
Now Python lives **on your computer**. You own the environment.

---

## Step 1 – Check if Python is already installed

Open Command Prompt:
- Press `Win + R`, type `cmd`, press Enter

Type this and press Enter:
```
python --version
```

**If you see something like `Python 3.12.1` → you're good. Skip to Step 3.**

If you see `'python' is not recognized` → go to Step 2.

---

## Step 2 – Install Python

1. Go to https://www.python.org/downloads/
2. Click **Download Python 3.x.x** (the big yellow button)
3. Run the installer
4. ⚠️ On the first screen: **check the box that says "Add Python to PATH"** — this is the most important step
5. Click **Install Now**
6. Close the installer when done

Now open a **new** Command Prompt window and run `python --version` again.

---

## Step 3 – Understand what you just installed

When you type `python` in the terminal, Windows looks through a list of folders (called PATH) to find the Python program. That's why checking "Add to PATH" matters — without it, Windows can't find Python.

Try these commands in Command Prompt:

```
python --version
```
Shows which Python version is installed.

```
python
```
Opens the **Python interactive shell** (REPL). You can type Python code line by line and it runs immediately. Try:
```python
>>> 2 + 2
>>> print("hello")
>>> exit()
```
Type `exit()` to get back to the normal terminal.

```
where python
```
Shows the file path where Python is installed on your machine.

---

## Step 4 – Check pip

`pip` is Python's package manager — you use it to install libraries. It comes with Python.

```
pip --version
```

You should see something like `pip 24.0 from C:\Users\...`

---

## ✅ Checklist before moving on

- [ ] `python --version` shows Python 3.10 or higher
- [ ] `pip --version` works
- [ ] You opened the Python REPL and ran a line of code
- [ ] You typed `exit()` to close it

Once all four are checked off, open `02_vscode_setup.md`.
