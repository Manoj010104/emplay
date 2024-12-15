# 🌟 RFP Document Data Extractor

## 📖 Overview

The **RFP Document Data Extractor** is a Python-based tool designed to extract structured information from Request for Proposal (RFP) documents in **PDF** and **HTML** formats. This program utilizes Natural Language Processing (NLP) techniques to identify and extract key fields from these documents, making it easier to analyze and process RFPs.

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

```bash
python -m spacy download en_core_web_sm
```

## 🛠️ Usage

1. **Prepare Your Documents**: Place your PDF and/or HTML files in a designated input folder.
2. **Run the Extractor**: Use the command line to execute the script, specifying the input folder and output file path:

```bash
python extract_rfp_data.py --input_folder path/to/input_folder --output_file path/to/output_file.json
```

3. **Check the Output**: The extracted data will be saved in the specified JSON file.

## 📄 Mock PDF Creation

For testing purposes, you can create a mock PDF file using the `generate_mock_pdf.py` script. This function generates a sample RFP document with predefined fields.

```bash
python generate_mock_pdf.py
```

## 💡 Example

To create a mock PDF and extract data from it, follow these steps:

```bash
# Create a mock PDF
python generate_mock_pdf.py

# Extract data from the created PDF
python extract_rfp_data.py --input_folder path/to/input_folder --output_file output.json
```

## 📂 File Descriptions

1. **extract_rfp_data.py**: Main Python script responsible for extracting structured information from RFP documents. It supports both PDF and HTML formats and utilizes NLP techniques.
2. **generate_mock_pdf.py**: Python script designed to create a mock PDF file for testing purposes. It generates a sample RFP document with predefined fields such as Bid Number, Title, Due Date, and more.
3. **output.json**: JSON file containing the structured information extracted from the RFP documents processed by the `extract_rfp_data.py` script. Each entry in the JSON file corresponds to a document processed.
4. **sample_rfp.html**: Sample HTML file that contains mock RFP data. It is used as an input document for the `extract_rfp_data.py` script. The HTML file includes various fields relevant to the RFP process.
5. **sample_rfp.pdf**: Sample PDF file that contains mock RFP data. Similar to the `sample_rfp.html` file, it is used as an input document for the `extract_rfp_data.py` script. The PDF includes various fields relevant to the RFP process.

## Installation

You can install the required packages using pip:

```bash
pip install spacy beautifulsoup4 PyPDF2 reportlab
```

---

