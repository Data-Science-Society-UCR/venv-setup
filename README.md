# virtual environment setup for MacOS/Windows

### Mac Installation

1. Install Python (There are a plethora of tutorials if you need them, but it should be pretty straightforward).
2. Open up `terminal`
3. To verify your Python installation and version enter the following command(s), depending on which one works.
```
python3 --version
```
```
python --version
```
4. CD to your Desktop, or wherever you want to store your project code.
5. Create a new directory named `venv`. This is the common naming notation for a virtual environment. If you prefer to organize your virtual environments by Python versions or projects you can reflect that in the naming like so: `venv_3_5_1` (for Python version 3.5.1) or `venv_ParkinsonML` for Parkinson's ML project. Do whatever works best for you!
6. To create the virtual environment, first you need to enter the directory. You can do this by using the `cd` command. The next step is in the virtual environment directory, enter one of the commands below, depending on which one works.
```
python3 -m venv .
```
```
python -m venv .
```
7. Type the following command `ls` to verify the creation of the virtual environment. You should see a few additional folders/files created (`bin`, `include`, `lib`, and `pyvenv.cfg`). Your directory might not look the same, however, it should look more or less similar.
8. To activate the virtual environment use the following command:
```
source bin/activate
```
9. We can now install the relevant libraries using the pip3/pip install function. Additionally, we can install Jupyter Notebook using the following command(s), depending on which one works:
```
pip3 install notebook
```
```
pip install notebook
```
10. After Jupyter Notebook is installed, you should be able to run it by typing `jupyter notebook` in the terminal.

### Windows Installation
1. 1. Install Python (There are a plethora of tutorials if you need them, but it should be pretty straight forward)
     * For Windows Users, make sure that Python is **added to your Path**. 
