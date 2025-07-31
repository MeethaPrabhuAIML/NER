# NER


# Project Title: Resume Information Extraction using NLP
## Objective
The main goal of this project is to build an automated resume parser that extracts structured information from unstructured resume documents (in PDF format). This task simulates a real-world HR automation scenario using Natural Language Processing (NLP) techniques and Named Entity Recognition (NER). The system focuses on identifying key fields such as Name, Email, Skills, Degree, Institution, and Work Experience from resumes.

## Tools and Libraries Used
Python – Core programming language.

pdfplumber – For extracting readable text content from PDF files.

NLTK (Natural Language Toolkit) – For natural language processing.

re (Regular Expressions) – For pattern-based entity extraction like email, degrees, and institutions.

json – To store structured data in a readable format.

## Workflow Summary
PDF Text Extraction
Using pdfplumber, each page of the PDF resume is read and converted into plain text.

Named Entity Recognition (NER)

Basic NER is performed using rule-based methods via NLTK and regex.

Person names are extracted based on context patterns and proper nouns.

Email addresses are captured using regex patterns.

Skill Extraction
A predefined list of technical skills (like Python, Java, TensorFlow, React, etc.) is matched against the resume text (case-insensitive match).

Degree and Institution Detection
Degree patterns like "B.Tech", "Masters", "Bachelor of..." are matched using regular expressions.
Institution names are extracted by identifying phrases that contain keywords like "College", "University", or "Institute".

Work Experience Section
Lines containing keywords like “intern”, “experience”, or similar terms are collected to form a brief experience summary.

Structured Output
All extracted entities are compiled into a dictionary and displayed in JSON format for easy storage or API usage.

## Sample Output
<img width="892" height="856" alt="image" src="https://github.com/user-attachments/assets/052af013-aaf7-448a-8902-3847222e4951" />
<img width="763" height="578" alt="image" src="https://github.com/user-attachments/assets/49d2e23d-7a11-4cdb-bc78-25c62bd241dc" />



## Key Benefits
Helps automate the resume screening process for HR and recruitment platforms.

Reduces manual effort and errors in parsing large volumes of resumes.

Can be integrated into applicant tracking systems (ATS) or web apps via APIs.

## Future Enhancements
Integrate a Streamlit UI for uploading resumes and displaying results interactively.

Add support for more advanced NER using SpaCy or Hugging Face Transformers.

Include multilingual resume parsing and image-based PDF OCR support.

Export parsed results to CSV or connect to cloud-based HR databases.
