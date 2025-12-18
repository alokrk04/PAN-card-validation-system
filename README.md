# PAN-card-validation-system
Completeed with cleaning and validating a dataset containing the Permanent Account Numbers (PAN) of Indian nationals. The goal is to ensure that each PAN number adheres to the official format and is categorised as either Valid or Invalid.


## PAN Number Validation Project

### Overview

This project focuses on the automated cleaning and validation of Indian **Permanent Account Numbers (PAN)**. Using a provided dataset, the objective is to ensure each entry adheres to the strict official format mandated for Indian nationals. The project involves complex data preprocessing and logical validation using either **Python or SQL**.

---

### Project Objectives

* 
**Data Cleaning**: Preprocess the dataset by handling missing values and removing duplicate entries.


* 
**Standardization**: Normalize data by removing leading/trailing spaces and converting all characters to uppercase.


* 
**Format Validation**: Implement logic to verify the 10-character alphanumeric structure.


* 
**Categorization**: Separate records into **Valid** and **Invalid** groups based on formatting rules.

---

### Validation Logic

A valid PAN must follow the specific pattern `AAAAA1234A`. This project implements the following refined rules:

1. **Prefix (First 5 Characters)**:
* Must be alphabetic uppercase letters.

* 
**No adjacent duplicates**: For example, `AABCD` is invalid.


* 
**No sequences**: Continuous sequences like `ABCDE` or `BCDEF` are prohibited.


2. **Numeric Part (Middle 4 Characters)**:
* Must be digits.

* 
**No adjacent duplicates**: For example, `1123` is invalid.

* 
**No sequences**: Continuous sequences like `1234` or `2345` are prohibited.

3. **Suffix (Last Character)**:
* Must be a single alphabetic uppercase letter.

---

### Deliverables

The final output includes a **Summary Report** providing the following metrics:

* Total records processed.


* Count of total valid vs. total invalid PANs.


* Count of missing or incomplete records.


---

### Tech Stack

**Language**: Python or SQL.

**Source Data**: Excel (`PAN Number Validation Dataset.xlsx`).
