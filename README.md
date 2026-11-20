# Unspupervised-Learning-For-Fraud-Detection_CSCI-3052U-Project

## About
The scope of this project is to determine if Unsupervised-learning methods can accurately detect credit card fraud.
It is very common that supervised learning is used for an issue as such,
but this project will compare and contrast the success of each method.

## Project Status
Dataset cleaning/filltering, data exploration and preprocessing. Training and testing strategy.

**Will be updated as we proceed with the project.*

## Dataset
**Dataset Name:**
CIS435 Credit Card Fraud Detection

**Source:** https://huggingface.co/datasets/dazzle-nu/CIS435-CreditCardFraudDetection

**License:** There was no specified license for this dataset.

## Repository Contents
- `model.ipynb`: Data exploration and preprocessing.
- `requirements.txt`: Libraries and depandancies needed for running the `model.ipynb` file.
- `fraudTrain.csv`: Dataset stored using Git LFS.

## Dataset Setup
Git LFS downloads the full dataset used by the notebook. In order to access the dataset, it must be installed on the users local computer

### macOS
If you use Homebrew, install Git LFS from Terminal:

```bash
brew install git-lfs
git lfs install
```

If you do not use Homebrew, download the macOS installer from [Git LFS](https://git-lfs.com/), install it, and run `git lfs install`.

### Windows
Download and run the Windows installer from the [official Git LFS releases](https://github.com/git-lfs/git-lfs/releases/latest). Reopen PowerShell after installation, then run:

```powershell
git lfs install
```

If Git LFS is already installed with Git for Windows, you only need to run `git lfs install`.

### Download the dataset (both platforms)
After cloning the repository, open Terminal or PowerShell in the project folder and run:

```bash
git lfs pull
```

This downloads `fraudTrain.csv` into the project folder beside `model.ipynb`. The notebook loads it using `pd.read_csv("fraudTrain.csv")`.

Make sure the CSV contains transaction rows rather than a short Git LFS pointer. If it contains only a few lines starting with `version https://git-lfs.github.com/spec/v1`, run `git lfs pull` again after installing Git LFS.

## Run the Notebook
Follow along with the steps below to run the notebook.

### 1. Create virtual environment
Open a terminal in the project folder, then run the commands for your platform to create and activate the virtual environment.

**Windows:**
```
py -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**Mac:**
```
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Install dependancies
Open a terminal in the project folder and run the following command to install the necessary libraries:

```
python -m pip install -r requirements.txt
```

### 3. Check the notebook kernel uses the virtual environment

If there is no indication of the kernel using the virtual enviromnemt created, follow along with the steps below.

In VS Code:

1. Open `model.ipynb`.

2. Select **Select Kernel** in the top-right corner of the notebook.

3. Choose **Python Environments**, then select the interpreter from this project's `.venv` folder:
   - **Windows:** `.venv\Scripts\python.exe`
   - **macOS:** `.venv/bin/python`
