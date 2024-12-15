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

### Installation

You can install the required packages using pip:

```bash
pip install spacy beautifulsoup4 PyPDF2 reportlab
