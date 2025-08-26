 ``
# Python Virtual Environment Setup on Kali Linux

This guide explains how to install and use `virtualenv` on Kali Linux to manage isolated Python environments for your projects.

---

## ✅ 1. Install `virtualenv`

```bash
sudo apt update
sudo apt install python3-virtualenv
````

Or using `pip`:

```bash
pip3 install virtualenv
```

---

## ✅ 2. Create a Project Folder (Optional)

```bash
mkdir myproject
cd myproject
```

---

## ✅ 3. Create a Virtual Environment

```bash
virtualenv venv
```

To specify a Python version:

```bash
virtualenv -p python3.11 venv
```

---

## ✅ 4. Activate the Virtual Environment

```bash
source venv/bin/activate
```

> You should now see `(venv)` in your terminal prompt.

---

## ✅ 5. Install Packages

```bash
pip install <package_name>
```

Example:

```bash
pip install requests
```

---

## ✅ 6. Check Installed Packages

```bash
pip list
```

---

## ✅ 7. Freeze Requirements (for sharing)

```bash
pip freeze > requirements.txt
```

---

## ✅ 8. Install from `requirements.txt`

```bash
pip install -r requirements.txt
```

---

## ✅ 9. Deactivate the Environment

```bash
deactivate
```

---

## 🔁 Example Flow

```bash
sudo apt install python3-virtualenv
mkdir myproject && cd myproject
virtualenv venv
source venv/bin/activate
pip install flask
deactivate
```

---

## 📁 Resulting Project Structure

```
myproject/
├── venv/
├── requirements.txt  # optional
```

---

Happy coding! 🐍

```

Let me know if you want this saved as a file or want a version with additional explanations or project examples.
```
