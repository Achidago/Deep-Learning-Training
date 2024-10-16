# Module 0 - Deep Learning Pre-Training Setup
## 1. Installing Python
### Windows
a. Download Python
   - Go to the [official Python website](https://www.python.org/downloads/)
   - Download the latest version (Python 3.9 or 3.10)

b. Install Python
   - Run the installer
   - Ensure that you check the box "Add Python to PaATH" during the installation process.
   - Click "Install Now"
  
c. Verify the installation
   - Open Command Prompt
   - Run python --version that Python is installed correctly. <br>

### MacOS
a. Install Homebrew (if not installed)
   - Open Terminal and run: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   - In the terminal run: brew install python

b. Install Python
   - Run python3 --version to ensure Python is installed.  <br> 


## 2. Installing Pip and Virtual Environment (Windows & macOS)

**Windows & macOS**  <br>

a. Upgrade pip
   - Windows: Open Command Prompt
   - macOS: Open Terminal
   - Run: python3 -m pip install --upgrade pip

b. Install virtual environment
   - Run: python3 -m pip install --user virtualenv

c. Create a virtual environment
   - Run: python3 -m venv myenv

d. Activate the virtual environment
   - On Windows: myenv\Scripts\activate
   - On macOS: source myenv/bin/activate


## 3. Installing TensorFlow

**Windows & macOS**  <br>

a. Activate the virtual environment (if not already activated)
   - Windows: myenv\Scripts\activate
   - macOS: source myenv/bin/activate

b. nstall TensorFlow
   - Run: pip install tensorflowv

c. Verify TensorFlow installation
   - Run the following in Python: import tensorflow as tf; print(tf.__version__)
   - This should print the TensorFlow version installed.


## 4. Installing PyTorch

**Windows & macOS**  <br>

a. Activate the virtual environment (if not already activated):
   - Windows: myenv\Scripts\activate
   - macOS: source myenv/bin/activate

b. Install PyTorch:
   - Go to the official PyTorch website and choose your configuration (Python, OS, CUDA/CPU).
   - Copy the recommended installation command and run it in your terminal/command prompt. For example: pip install torch torchvision torchaudio

c. Verify TensorFlow installation:
   - Run the following in Python: import torch; print(torch.__version__)
   - This should print the PyTorch version installed.
 

## 5. Exercises and Pre-training Survey

- Please complete the [[Exercise 0]]

- Please submit your exercises [[here]](https://github.com/SERVIR-WA/GALUP/issues/new?assignees=Achidago&labels=Exercise+W4M0&template=Exercise0Template.md&title=Workshop+4+exercise+0+%5Breplace+with+your+name%5D)

## 6. What's Next?

Module 1 - [Time Series Analysis](module1.md)

## 8. Other Resources


