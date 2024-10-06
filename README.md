# Discourse-Analysis-Tool
A Python-based discourse analysis tool that compares written and spoken texts using linguistic elements like grammatical complexity, lexical diversity, interactive features, speech markers, and formal vocabulary use.
# Discourse Analysis Using Python in Google Colab

This project provides a Python-based analysis tool for both written and spoken discourse. The program analyzes linguistic features using specific elements across different discourse types. It compares and contrasts these discourses based on a set of predefined linguistic factors, providing meaningful visualizations and metrics for better understanding of the linguistic differences between them. This project was implemented in Google Colab and requires authentication with Google Drive to access files.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Linguistic Factors Analyzed](#linguistic-factors-analyzed)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Notes](#notes)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The primary purpose of this project is to compare written and spoken discourse using seven key linguistic factors. The analysis includes metrics such as grammatical complexity, lexical diversity, interactive features, and speech markers. The data is gathered from two MS Word documents: **Written Discourse** and **Spoken Discourse**. These files are retrieved from Google Drive, analyzed, and presented using tabular results.

## Features
- Extracts text from MS Word files for analysis.
- Analyzes linguistic features like grammatical complexity, lexical diversity, interactive features, and more.
- Uses Google Colab for easy execution in a cloud environment.
- Retrieves files from Google Drive and performs linguistic analysis without needing manual file uploads.
- Saves the final results in a CSV file.

## Linguistic Factors Analyzed
The program focuses on the following linguistic factors and elements for analysis:
1. **Grammatical Complexity**
   - **Passive Voice Construction**: Counts the number of passive constructions in the text.
   - **Sentence Length**: Calculates the average sentence length.

2. **Lexical Diversity**
   - **Type-Token Ratio (TTR)**: Measures lexical diversity by comparing the number of unique tokens to the total number of tokens.
   - **Average Word Length**: Calculates the average length of words in the text.

3. **Interactive Features**
   - **Questions Count**: Counts the number of questions in the text.
   - **Imperative Verbs**: Counts the number of imperative verbs.

4. **Speech Markers**
   - **Discourse Markers**: Analyzes the use of discourse markers (e.g., "well", "like", "you know").

5. **Formal Vocabulary Use**
   - **Formal Vocabulary**: Analyzes the frequency of formal terms used in the discourse.

## Installation
The project requires Python 3 and is designed to run on Google Colab. Google Colab provides an ideal environment with many pre-installed dependencies, making it easier to set up.

1. **Clone the repository**: You can start by cloning the repository to your local machine.
   ```bash
   git clone <repository-link>
   ```

2. **Upload to Google Colab**: Open the `.ipynb` file in Google Colab.

## Running the Project
1. Open the `.ipynb` file in Google Colab.
2. Make sure you authenticate with Google Drive by following the prompts.
3. Replace the Google Drive File IDs with your own if you wish to use custom files for analysis.
4. Run all the cells to execute the analysis and generate the CSV results.

## Dependencies
The following Python packages are required:
- `nltk`: Used for tokenization, sentence segmentation, and other natural language processing tasks.
- `spacy`: Used to analyze syntactic dependencies for passive construction detection.
- `docx`: To read MS Word documents.
- `google-api-python-client`: To connect and retrieve files from Google Drive.
- `pandas`: For managing and analyzing data.
- `matplotlib` and `seaborn`: For visualizing the results.

The installation of these packages is handled by the `!pip install` commands at the beginning of the notebook.

## Usage
- The program first authenticates with Google Drive to download the discourse files.
- The files should be named "Written_Discourse" and "Spoken_Discourse" in `.docx` format.
- The linguistic analysis is performed, focusing on different factors and elements to distinguish the written from the spoken discourse.
- The output includes a CSV file with the analyzed features.

### Google Drive File Access
To analyze your files, make sure they are stored in Google Drive, and use their respective file IDs in the code. Google Colab requires authentication to access Google Drive, so each time you run the notebook, you will need to authenticate.

### Analysis Results
The results are saved in a CSV file called `discourse_analysis_refined_results.csv`. The CSV contains the following columns:
- **Serial Number**: Index for the result.
- **Linguistic Factor**: The factor being analyzed.
- **Element**: Specific element of the factor analyzed.
- **Words Analyzed**: The words or phrases counted/considered.
- **Value**: The value calculated for the element.

## Project Structure
- **discourse_analysis.ipynb**: The main code file where the analysis is performed.
- **discourse_analysis_refined_results.csv**: The results file generated after executing the notebook.
- **README.md**: Documentation and instructions for using the project.

## Notes
- Ensure you use your own Google Drive file IDs.
- Google authentication is required every time you run the notebook in Colab.
- For public sharing, avoid exposing sensitive information like file IDs or Google credentials.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request if you wish to improve the analysis or add more linguistic factors.

1. Fork the project.
2. Create your feature branch (`git checkout -b feature/NewFeature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/NewFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

Feel free to reach out if you have any questions or suggestions for improvement!

