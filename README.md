# Resume Summarization and Comparison System

Welcome to the **Resume Summarization and Comparison System**! This project allows you to summarize and compare resumes using Google's Gemini AI model. The program reads PDF files, summarizes their content based on education, projects, experience, and certifications/achievements, and even compares two resumes to suggest which candidate might be the best to hire.

## Features

- **Summarize Resume**: Summarize the content of a resume based on key factors like education, projects, experience, and certifications.
- **Compare Resumes**: Compare two resumes and get an AI-based suggestion on which candidate might be better to hire.

## Requirements

To run this project, you'll need to have the following packages installed:

- `google-generativeai`: To interact with the Google Gemini AI model.
- `PyMuPDF`: To read and extract text from PDF files.

You can install these dependencies using the following commands:

```bash
pip install -U -q google-generativeai
pip install PyMuPDF
```
## How to Use

### 1. Setting Up the API Key
First, configure the Google Gemini AI API key:

```python
import google.generativeai as genai

GOOGLE_API_KEY = "YOUR_API_KEY"  # Replace with your API Key
genai.configure(api_key=GOOGLE_API_KEY)
```
### 2. Summarizing a Resume
To summarize a resume, place the PDF file in your desired location and run the program. Choose the "Summarize Resume" option and provide the file's location:

```python
location = "path/to/your/resume.pdf"
print(summarize_resume(location))
```
### 3. Comparing Two Resumes
To compare two resumes, place the PDF files in your desired locations and choose the "Compare Resumes" option. Provide the locations of both files:

```python
location1 = "path/to/first/resume.pdf"
location2 = "path/to/second/resume.pdf"
print(compare_resume(location1, location2))
```
### 4. Running the Program
The program provides a simple command-line interface:

- Choose `1` to summarize a single resume.
- Choose `2` to compare two resumes.

```bash
Welcome to the Resume Summarization and Comparing System!
Kindly enter the operation that you want to perform...
1. Summarize the Resume.
2. Compare 2 Resume.
Enter your choice: 
```
### 5. Error Handling
The program includes basic error handling to ensure smooth execution. If an error occurs, the user is informed, and they can choose to rerun the program.

### Conclusion
This project is an excellent tool for anyone looking to quickly summarize or compare resumes using AI. Whether you're an HR professional, recruiter, or just someone interested in AI-driven tools, this system provides a quick and efficient way to analyze resumes.

Feel free to contribute to this project by adding new features or improving existing ones!
