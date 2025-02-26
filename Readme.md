# Setting Up a Local Environment with Anaconda/Miniconda

This guide walks you through installing Anaconda or Miniconda and setting up a Python environment on your local machine to try out code.

## Step 1: Install Anaconda or Miniconda
1. **Download**:
   - **Anaconda**: Get it from [https://www.anaconda.com/products/distribution](https://www.anaconda.com/products/distribution). Choose the version for your operating system (Windows, macOS, or Linux).
   - **Miniconda**: Download from [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html). Pick the installer matching your OS.
2. **Install**:
   - **Windows**: Double-click the `.exe` file and follow the installer prompts. Default settings are usually fine but make sure to note the installation path and select the option to add Conda to your PATH if prompted.
   - **macOS/Linux**: Open a terminal, navigate to the download location (e.g., `cd ~/Downloads`), and run the script (e.g., `bash Miniconda3-latest-Linux-x86_64.sh`). Follow the prompts.
3. **Verify**:
   - Open a terminal (or Anaconda Prompt on Windows).
   - Type `conda --version`. You should see output like `conda 23.7.4`. If not, troubleshoot your installation.

## Step 2: Open Anaconda Prompt (or Terminal)
- **Windows**: Search for "Anaconda Prompt" in the Start menu and open it.
- **macOS/Linux**: Use your regular terminal after installation (Miniconda doesn’t come with a separate prompt).
- This is where you’ll run `conda` commands.

## Step 3: Create a Conda Environment
To create an environment with dependencies listed in a `requirements.txt` file:
1. Ensure you have a `requirements.txt` file in your current directory. This file should list packages and versions (e.g., `numpy==1.21.0`).
2. Run the following command in the Anaconda Prompt (or terminal):
- conda create --name myenv --file requirements.txt or conda create --name myenv --file requirements.txt -c conda-forge -c defaults
- Replace `myenv` with your desired environment name (e.g., `data_science`).
## Step 5: Run Your Code
- With the environment activated, you can now run your Python scripts
