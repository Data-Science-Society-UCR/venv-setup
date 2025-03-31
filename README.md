# virtual environment setup for MacOS/Windows

## Mac Installation

### 1. Install Python
If you haven't already installed Python, install it from the official website: https://www.python.org/downloads/

### 2 & 3. Open Terminal and Verify Python Installation
Check if Python is installed by running one of the following commands:
```
python3 --version
```
```
python --version
```
If neither works, you may need to install Python or check your PATH settings.

### 4. Clone the Repository
Navigate to the location where you want to store your project using the `cd` command (e.g., `cd ~/Desktop`)

Clone the Repo using the repo's HTTPS:
```
git clone https://github.com/your-username/your-repo.git
```

Navigate into the project directory
```
cd your-repo-name
```

### 5. Create a Virtual Environment Inside the Repository
Use one of the following commands, depending on which one works.
```
python3 -m venv venv
```
```
python -m venv venv
```
This will create a `venv/` directory inside the repository. 

### 6. Activate the Virtual Environment
Run the following command to activate the virtual environment:
```
source venv/bin/activate
```

### 7. Install Project Dependencies
If the repository has a `requirements.txt` file, install dependencies (Please note, that not every DSS project will have a `requirements.txt`):
```
pip3 install -r requirements.txt
```
```
pip install -r requirements.txt
```

Additionally, you may want to verify the installed packages using the `pip3 list`/`pip list` command.

### 8. Add Virtual Environment to `.gitignore`
To prevent accidentally committing the virtual environment, create a git ignore using the `touch` command, and add the following line to the `.gitignore` (the file name must be .gitignore)!.
```
venv/
```

### 9. Run Jupyter Notebook (May differ depending on the project requirements)
```
pip3 install notebook
```
```
pip install notebook
```
And to run Jupyter Notebook use the following command:
```
jupyter notebook
```

### 10. Deactive the Virtual Environment When Done
```
deactivate
```

## Windows Installation
1. 1. Install Python (There are a plethora of tutorials if you need them, but it should be pretty straight forward)
     * For Windows Users, make sure that Python is **added to your Path**. 
