# SMS Text Classification Interface

This project implements a simple SMS spam detection system using machine learning and provides a user-friendly web interface built with Gradio.

## Description

The application uses a Linear Support Vector Classification model with TF-IDF vectorization to classify SMS messages as either spam or non-spam ("ham"). The interface allows users to input any text message and receive an immediate classification result.

## Prerequisites

Before running this application, ensure you have the following installed:
- Python 3.10 or later
- Jupyter Notebook
- Required Python packages:
  - pandas
  - scikit-learn
  - gradio

## Installation

1. Clone this repository or download the files to your local machine
2. Install the required packages using pip:
```bash
pip install pandas scikit-learn gradio jupyter
```

## Dataset

The application uses the SMSSpamCollection dataset. Ensure the dataset file is placed in the following location:
- `Resources/SMSSpamCollection.csv`

## Running the Application

1. Navigate to the project directory
2. Launch Jupyter Notebook:
```bash
jupyter notebook
```
3. Open `gradio_sms_text_classification.ipynb`
4. Run all cells in the notebook sequentially (Cell → Run All)
5. The Gradio interface will launch automatically in the notebook
6. You can now enter text messages to test if they are classified as spam or not

## Usage

1. Once the interface is running, you will see a text input box
2. Enter any SMS message you want to classify
3. The system will immediately respond with whether the message is classified as spam or not

## Example Messages to Test

Try these example messages to test the system:
- "You are a lucky winner of $5000!"
- "You won 2 free tickets to the Super Bowl."
- "You won 2 free tickets to the Super Bowl text us to claim your prize."
- "Thanks for registering. Text 4343 to receive free updates on medicare."

## Model Details

The classification system uses:
- TF-IDF (Term Frequency-Inverse Document Frequency) vectorization
- Linear Support Vector Classification
- 67/33 train-test split ratio