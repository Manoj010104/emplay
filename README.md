# 🌟 RFP Document Data Extractor

## 📖 Overview

The **RFP Document Data Extractor** is a powerful Python tool designed to extract structured data from Request for Proposal (RFP) documents in **PDF** and **HTML** formats. Leveraging the capabilities of the **spaCy** NLP library for entity recognition and regular expressions for field extraction, this tool simplifies the process of gathering essential information from RFPs.

## 🚀 Features

- **Key Field Extraction**: Automatically extracts important fields, including:
  - **Bid Number**
  - **Title**
  - **Due Date**
  - **Payment Terms**
  - **Contact Information**
  - **Company Name**
- **File Format Support**: Works with both **PDF** and **HTML** documents.
- **Structured Output**: Saves extracted data in a clean and organized **JSON** format.

## 📦 Requirements

To run this project, you will need:

- **Python 3.6 or higher**
- Required Python packages:
  - `spacy`
  - `beautifulsoup4`
  - `PyPDF2`
  - `reportlab`

### Installation

You can install the required packages using pip:

```bash
pip install spacy beautifulsoup4 PyPDF2 reportlab
