# Step-by-Step Installation Guide for Beginners

## What You Need

Before starting, make sure you have:
1. **A computer** (Windows, Mac, or Linux)
2. **An internet connection**
3. **Admin/user access** to install software
4. **(Optional but recommended) An NVIDIA GPU** for faster performance

---

## Step 1: Install Python

### Windows
1. Go to https://www.python.org/downloads/
2. Click the big yellow "Download Python 3.x.x" button
3. Run the installer
4. **IMPORTANT:** Check the box that says "Add Python to PATH"
5. Click "Install Now"

### macOS
1. Go to https://www.python.org/downloads/
2. Download the macOS installer
3. Run it and follow the prompts

### Linux
Open terminal and run:
```bash
sudo apt-get update
sudo apt-get install python3 python3-pip
```

**Verify installation:**
```bash
python --version
```
Should show Python 3.8 or higher.

---

## Step 2: Install Git

### Windows & macOS
1. Go to https://git-scm.com/
2. Download and run the installer
3. Follow default settings

### Linux
```bash
sudo apt-get install git
```

**Verify installation:**
```bash
git --version
```

---

## Step 3: Clone This Repository

Open Command Prompt (Windows) or Terminal (Mac/Linux) and run:

```bash
git clone https://github.com/jromjenine76-alt/wan2gp-notebook.git
cd wan2gp-notebook
```

---

## Step 4: Create a Virtual Environment

A virtual environment keeps your project packages separate from your system.

### Windows
```bash
python -m venv venv
venv\Scripts\activate
```

### macOS/Linux
```bash
python3 -m venv venv
source venv/bin/activate
```

**If successful, you should see `(venv)` at the start of your terminal line.**

---

## Step 5: Install Required Packages

```bash
pip install -r requirements.txt
```

This will take 10-30 minutes depending on your internet speed. Let it finish completely.

---

## Step 6: Run the Notebook

Once installation completes, start Jupyter:

```bash
jupyter notebook
```

A browser window will open. Click on the notebook file (`.ipynb`) to open it.

---

## Troubleshooting

### "Python command not found"
- **Windows:** Make sure you checked "Add Python to PATH" during installation
- **Reinstall Python** and check the PATH box

### "pip command not found"
- Try `pip3` instead of `pip`

### Installation taking too long
- This is normal! GPU packages can be large. Just wait.

### "No module named 'torch'"
- Make sure your virtual environment is activated (you see `(venv)` in terminal)

### "CUDA not available" (GPU error)
- You need an NVIDIA GPU and CUDA Toolkit installed
- For now, the code will still run on CPU, just slower

---

## Need More Help?

1. **Check the README.md** for general info
2. **Google the error message** - most common errors have solutions
3. **Ask on GitHub Issues** in this repository

You've got this! 🚀
