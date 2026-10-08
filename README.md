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

## Run the Notebook
Follow along with the steps below to run the notebook.

### 1. Create virtual environment
Run the following commands within a terminal to acitvate the virtual environment.

**Windows:**
```
cd \Unspupervised-Learning-For-Fraud-Detection_CSCI-3052U-Project"
```
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