  **uv simple setup** of the commands for using `uv` to manage Python projects, tailored for Windows users and focused only on essential steps:

---

### **1. Install `uv`**  
Run this in **PowerShell** to install `uv` on Windows:  
```powershell
irm https://astral.sh/uv/install.ps1 | iex
```

---

### **2. Create a New Project**  
To create a new project, run:  
```powershell
uv init example
cd example
```

---

### **3. Add a Dependency**  
To add a dependency (e.g., `ruff` for linting), use:  
```powershell
uv add ruff
```

---

### **4. Run a Command in the Project**  
Run commands or scripts in the project environment. For example, to check your project files with `ruff`:  
```powershell
uv run ruff check
```

---

### **5. Add Another Dependency (Optional)**  
If you want to add more dependencies later (e.g., `requests`):  
```powershell
uv add requests
```

---

### **6. Run Python Scripts**  
You can also run Python scripts using `uv`. Example:  
1. Create a script called `example.py` with this content:  
   ```python
   import requests

   response = requests.get("https://jsonplaceholder.typicode.com/todos/1")
   print(response.json())
   ```
2. Run it:  
   ```powershell
   uv run example.py
   ```

---

### **Folder Structure Created by `uv`**  
After initializing a project, `uv` will create these files:  
```
.
├── .venv               # Virtual environment for dependencies
├── .python-version     # Python version for the project
├── pyproject.toml      # Project metadata and dependencies
├── uv.lock             # Locked dependency versions
├── README.md           # Placeholder for project documentation
├── example.py          # Example script created during initialization
```

---

This step-by-step guide is tailored to help students focus only on essential commands and processes, keeping things simple and clear. 
