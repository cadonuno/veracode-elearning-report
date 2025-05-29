# Veracode eLearning Users Report

## Requirements:
- Python 3.12+ (https://www.python.org/downloads/)
- API Credentials generated from a Veracode account with the eLearning permission and set as an eLearning Manager
    - To obtain API credentials for your user account, you can follow this article: https://docs.veracode.com/r/c_api_credentials3

## Installation

This repository contains a script to construct a Veracode eLearning users completion status report in Excel format. 

Clone this repository:

    git clone https://github.com/cadonuno/veracode-elearning-report

Install dependencies:

    cd veracode-elearning-report
    pip install -r requirements.txt

(Optional) Save Veracode API credentials in `~/.veracode/credentials`

    [default]
    veracode_api_key_id = <YOUR_API_KEY_ID>
    veracode_api_key_secret = <YOUR_API_KEY_SECRET>

## Run

If you have saved credentials as above you can run:

    python veracode-elearning-report.py -f eLearningReport.xlsx

Otherwise you will need to set environment variables:

    export VERACODE_API_KEY_ID=<YOUR_API_KEY_ID>
    export VERACODE_API_KEY_SECRET=<YOUR_API_KEY_SECRET>
    python veracode-elearning-report.py -f eLearningReport.xlsx


If all went well, the above command will create a new file called `eLearningReport.xlsx` which you can open with Excel.

> ___Note___ - depending on your environment, you may need to use `pip3` instead of `pip` and `python3` instead of `python`.
