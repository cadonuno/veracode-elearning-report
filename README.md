# Veracode eLearning Users Report

This repository contains a script to construct a Veracode eLearning users completion status report in Excel format. 

## Prerequisites

### Python
the script is written in Python and require that you have a Python installed on your PC

You can check that by typing `python --version` in your command prompt or terminal

If you don't get a result of the installed Python version, please install Python on your PC. You can find the installation here: https://www.python.org/downloads/

### Veracode API Credentials

In order to query for the information for the report the script requires access to the Veracode platform. The script assumes you already have a user account and setup API credentails which are stored in your local computer.

If you do not have Veracode API credentials setup on your PC which runs the script, please follow these instructions: [Setting local API Credentials](https://docs.veracode.com/r/c_api_credentials3)

<a id="installation"></a>
## Installation and Report Generation

To run this script you first need to install the required packages that support the script with the following command.

`pip install -r requirements.txt`

Once all packages installed, use this python command to execute the main script file in this repository

`python ./veracode-elearning-report.py -f eLearningReport.xlsx`

You'll see prompt of the different calls to the Veracode platform to query the information need to construct the report.

If all went well, the above command will create a new file `eLearningReport.xlsx` which you can open with Excel.

> ___Note___ - depending on your environment, you may need to use `pip3` instead of `pip` and `python3` instead of `python` if the above commands do not work for you
