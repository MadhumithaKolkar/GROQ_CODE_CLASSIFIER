# Code vs Non-Code Classifier with Groq and Gradio

## Overview

This project implements a web-based interface using Gradio for classifying and chunking text into code and non-code segments. It leverages the `Llama3` model via the Groq API to process input text and provide classifications. The web interface allows users to input text and receive an organized output that separates code and non-code segments, as well as an overall classification of the input text.

## Features

- **Text Classification**: Uses `Llama3` via Groq API to classify lines of text as "Code" or "Non-Code."
- **Text Chunking**: Separates the input text into chunks based on the classification, grouping similar lines together.
- **Formatted Output**: The output is formatted with proper indentation to distinguish between code and non-code chunks.
- **Web Interface**: Powered by Gradio, the interface allows for easy interaction with the classifier.

## Requirements

- Python 3.7 or higher
- The following Python packages:
  - `gradio`
  - `groq` (Groq's API client)
  
  Install the dependencies using the following command:
  
  ```bash
  pip install gradio groq

Groq API Key: You need to have a Groq API key to use the Llama3 model. Replace the placeholder in the code with your actual API key.

## Usage

Clone the Repository:

git clone https://github.com/your-repository/code-vs-non-code-classifier.git
cd code-vs-non-code-classifier

Set Up API Key:
Replace the placeholder in the code with your actual Groq API key:

GROQ_API_KEY = 'your_api_key_here'

Run the Application:
Execute the notebook to launch the Gradio interface:

The interface will be accessible through your notebook.

Classify Text:
Enter text in the provided textbox and click "Submit." The output will show the separated code and non-code chunks, along with an overall classification of the input.

## Code Structure

classify_text_with_llama3: Function that classifies a single line of text using the Llama3 model.
chunk_text_with_llama3: Splits the input text into code and non-code chunks.
classify_and_process: Processes the entire input to classify and chunk it, and determines the overall status.
format_output: Formats the chunks for better readability in the output.
process_text: Main function that integrates all the other functions and returns the final formatted result.
Gradio Interface: Configures and launches the Gradio interface for user interaction.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For any issues or questions, please feel free to reach out to Madhumitha Kolkar.
