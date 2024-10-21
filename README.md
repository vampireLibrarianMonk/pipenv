# Pipenv Installation and Configuration

### 1. Install pip for Python:
If `pip` is not already installed, use the following command to install it:
```bash
sudo apt-get install python3.x-distutils
wget https://bootstrap.pypa.io/get-pip.py
python3.x get-pip.py
```

### 2. Install pipenv via pip:
Once `pip` is installed, you can install `pipenv` by running:
```bash
python3.x -m pip install --user pipenv
```

### 3. Add pipenv to your PATH (if necessary):
To make sure `pipenv` is globally accessible, add it to your PATH:
```bash
export PATH="$HOME/.local/bin:$PATH"
```

To persist this change across terminal sessions, add the above line to your `.bashrc` or `.zshrc`:
```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

### 4. Create a Virtual Environment with pipenv:
Navigate to your project directory and run the following command to create a virtual environment using pipenv:
```bash
pipenv --python 3.x
```
Replace `3.x` with the Python version you want to use for the environment.

### 5. Install Packages in the Virtual Environment:
You can install Python packages into the pipenv environment with:
```bash
pipenv install <package-name>
```

### 6. Activate the Virtual Environment:
To activate the pipenv environment, use:
```bash
pipenv shell
```

### 7. Deactivate the Environment:
When you are done working in the virtual environment, you can deactivate it with:
```bash
exit
```
