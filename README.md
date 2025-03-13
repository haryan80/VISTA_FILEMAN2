
# VISTA FILAMAN - VistA Vitals Data Extraction Tool

## Overview
This project contains a Jupyter notebook (`pyodbc-vitals.ipynb`) designed to extract vital signs data from a VistA/WorldVistA EHR system and store it in a local database. The tool connects to the VistA system via SSH, extracts vital signs data, and then processes and stores this information for further analysis.

## Features
- Secure SSH connection to VistA system
- Automated login and navigation through VistA terminal interface
- Extraction of patient vital signs data
- Data parsing and transformation
- Storage in a local SQL database
- Scheduled execution with configurable intervals

## Requirements
- Python 3.x
- Required Python packages:
  - pyodbc
  - pandas
  - tqdm
  - paramiko
  - cryptography
  - python-dotenv

## Setup
1. Ensure all required Python packages are installed
2. Configure your environment variables in a `.env` file with:
   - VistA server credentials
   - Database connection details
   - File paths for data storage

## Usage
1. Open the `pyodbc-vitals.ipynb` notebook in Jupyter
2. Run the cells in sequence to:
   - Connect to the VistA system
   - Extract vital signs data
   - Process and store the data
   - Schedule recurring extractions

## Security Notes
- The notebook includes encryption for sensitive credentials
- Always follow your organization's security policies when handling patient data
- Ensure proper access controls are in place for the extracted data

