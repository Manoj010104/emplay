# 🌟 RFP Document Data Extractor

## 📖 Overview

The **RFP Document Data Extractor** is a Python-based tool designed to extract structured information from Request for Proposal (RFP) documents in **PDF** and **HTML** formats. This program utilizes **Natural Language Processing (NLP)** techniques, including **spaCy**, to accurately interpret and extract relevant data from various document structures.

## 🚀 Features

- **Key Field Extraction**: Automatically extracts important fields, including:
  - **Bid Number**
  - **Title**
  - **Due Date**
  - **Bid Submission Type**
  - **Term of Bid**
  - **Pre Bid Meeting**
  - **Installation**
  - **Bid Bond Requirement**
  - **Delivery Date**
  - **Payment Terms**
  - **Any Additional Documentation Required**
  - **MFG for Registration**
  - **Contract or Cooperative to use**
  - **Model_no**
  - **Part_no**
  - **Product**
  - **Contact Info**
  - **Company Name**
  - **Bid Summary**
  - **Product Specification**
  - **Value**
- **File Format Support**: Processes both **PDF** and **HTML** documents.
- **Structured Output**: Saves extracted data in a clean and organized **JSON** format.

## 📦 Requirements

To run this project, you will need:

- **Python 3.6 or higher**
- Required Python packages:
  - `spacy`
  - `beautifulsoup4`
  - `PyPDF2`
  - `reportlab`

Make sure to download the spaCy language model:

bash

Verify

Open In Editor
Run
Copy code
python -m spacy download en_core_web_sm
🛠️ Usage
Prepare Your Documents: Place your PDF and/or HTML files in a designated input folder.

Run the Extractor: Use the command line to execute the script, specifying the input folder and output file path:

bash

Verify

Open In Editor
Run
Copy code
python extract_rfp_data.py --input_folder path/to/input_folder --output_file path/to/output_file.json
Check the Output: The extracted data will be saved in the specified JSON file.

📄 Mock PDF Creation
For testing purposes, you can create a mock PDF file using the generate_mock_pdf.py script. This function generates a sample RFP document with predefined fields.

bash

Verify

Open In Editor
Run
Copy code
python generate_mock_pdf.py
💡 Example
To create a mock PDF and extract data from it, follow these steps:

bash

Verify

Open In Editor
Run
Copy code
# Create a mock PDF
python generate_mock_pdf.py

# Extract data from the created PDF
python extract_rfp_data.py --input_folder path/to/input_folder --output_file output.json
📂 File Descriptions
1. extract_rfp_data.py
This is the main Python script responsible for extracting structured information from RFP documents. It supports both PDF and HTML formats and utilizes Natural Language Processing (NLP) techniques, specifically the spaCy library, to identify and extract relevant fields from the documents. The extracted data is then organized into a predefined structure and saved in a JSON format.

2. generate_mock_pdf.py
This Python script is designed to create a mock PDF file for testing purposes. It generates a sample RFP document with predefined fields such as Bid Number, Title, Due Date, and more. This mock PDF can be used to test the functionality of the extract_rfp_data.py script without needing real RFP documents.

3. output.json
This JSON file contains the structured information extracted from the RFP documents processed by the extract_rfp_data.py script. Each entry in the JSON file corresponds to a document processed, with fields such as Bid Number, Title, Due Date, and others filled with the extracted data. This file serves as the output of the extraction process and can be used for further analysis or reporting.

4. sample_rfp.html
This is a sample HTML file that contains mock RFP data. It is used as an input document for the extract_rfp_data.py script. The HTML file includes various fields relevant to the RFP process, allowing users to test the extraction functionality of the program.

5. sample_rfp.pdf
This is a sample PDF file that contains mock RFP data. Similar to the sample_rfp.html file, it is used as an input document for the extract_rfp_data.py script. The PDF includes various fields relevant to the RFP

### Installation

You can install the required packages using pip:

```bash
pip install spacy beautifulsoup4 PyPDF2 reportlab
