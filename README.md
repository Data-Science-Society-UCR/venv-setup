# virtual environment setup for MacOS/Windows

![macOS](https://img.shields.io/badge/macOS-Virtual%20Environment%20Setup-000000?style=for-the-badge&logo=apple)
![Windows](https://img.shields.io/badge/Windows-Virtual%20Environment%20Setup-0078D4?style=for-the-badge&logo=microsoft)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Virtual Environment](https://img.shields.io/badge/Virtual%20Environment-venv-%234CBB87?style=for-the-badge)
![Dependencies](https://img.shields.io/badge/Dependencies-Requirements%20File-%23FFD700?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-Version%20Control-F05032?style=for-the-badge&logo=git&logoColor=white)
![Homebrew](https://img.shields.io/badge/Homebrew-Package%20Manager-FBB040?style=for-the-badge&logo=homebrew&logoColor=white)

### NOTE: For this workflow, you need to have Git installed. If you do not have these programs installed, please use the following links.
Git can be installed via Brew on MacOS:
[Git Website](https://git-scm.com/downloads/mac), [Brew Website](https://brew.sh/), [How to install Brew on Mac (video)](https://www.youtube.com/watch?v=flQxyoyBX5M)

To install Git on Windows, use the following documentation and go to the section "[Installing on Windows](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)"


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

Clone the Repo using the repo's HTTPS (the HTTPS can be found by going to the Repo webpage, clicking the green code button clicking the `HTTPS` tab, and copying the web URL):
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
To prevent accidentally committing the virtual environment, create a git ignore using the `echo` command (if it does not already exist), and add the following line to the `.gitignore` (the file name must be .gitignore)! You can achieve this by using the following command:
```
echo 'venv/' >> .gitignore
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

We will go more into depth about the git-workflow when the projects begin, but this setup will be sufficient and put the entire team(s) on the same page.

## Windows Installation

### 1. Install Python
If you haven't already installed Python, install it from the official website: https://www.python.org/downloads/

### 2. Open PowerShell or Command Prompt

### 3. Verify Python Installation
```
python --version
```

### 4. Clone the repository using HTTPS 
Navigate to the location where you want to store your project using the `cd` command (e.g., `cd ~/Desktop`)

Clone the repo using HTTPS (The HTTPS can be found by going to the Repo webpage, clicking the green code button clicking the `HTTPS` tab, and copying the web URL).
```
git clone https://github.com/your-username/your-repo.git
```

Navigate into the project directory.
```
cd your-repo-name
```

### 5. Create a Virtual Environment Inside the Repository
```
python -m venv venv
```

### 6. Activate the Virtual Environment
* Command Prompt:
```
.venv\Scripts\activate
```
* PowerShell
```
.venv\Scripts\Activate.ps1
```

### 7. Install Project Dependencies
```
pip install -r requirements.txt
```

Additionally, you may want to verify the installed packages using the `pip list` command.

### 8. Add Virtual Environment to `.gitignore`
To prevent accidentally committing the virtual environment, create a git ignore using the `echo` command (if it does not already exist), and add the following line to the `.gitignore` (the file name must be .gitignore)! You can achieve this by using the following command:
```
echo venv/ > .gitignore
```

### 9. Run Jupyter Notebook (May differ depending on the project requirements)
```
pip install notebook
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
