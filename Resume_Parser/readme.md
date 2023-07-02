# Resume Parser NLP

This repository contains code and resources for a Resume Parser using Natural Language Processing (NLP) techniques. The Resume Parser is designed to extract relevant information from resumes automatically, such as contact details, skills, education, work experience, and more. By leveraging NLP, this tool can save time and effort in processing a large number of resumes during recruitment processes.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Methods](#methods)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

To use the Resume Parser NLP tool, you need to follow these installation steps:

1. Clone the repository to your local machine by executing the following command:

    ```
    `git clone https://github.com/jhonny1677/Resume_Parser_NLP.git`
    ```

2. Ensure you have Python 3.x and pip installed on your system.

3. Install the required dependencies by running the following command:

    ```
    `pip install -r requirements.txt`
    ```

4. Download the necessary NLTK corpora by executing the following command:

    ```
    `python -m nltk.downloader stopwords`
    `python -m nltk.downloader punkt`
    `python -m nltk.downloader averaged_perceptron_tagger`
    ```

5. Make sure you have compatible language models for the NER (Named Entity Recognition) algorithm. Refer to the [spaCy documentation](https://spacy.io/models) for more information on downloading and installing models.

## Usage

After completing the installation steps, you can use the Resume Parser NLP tool as follows:

1. Prepare your resumes in PDF format and place them in the `resumes` directory.

2. Run the `resume_parser.py` script to start the parsing process:

    ```
    `python resume_parser.py`
    ```

3. The script will process all the resumes in the `resumes` directory and extract the relevant information.

4. The parsed information will be saved as JSON files in the `output` directory.

5. You can customize the output format and fields in the `resume_parser.py` script based on your requirements.

## Data

The resumes to be parsed should be placed in the `resumes` directory. Make sure the resumes are in PDF format for accurate parsing. You can add or remove resumes from this directory as needed.

## Methods

The Resume Parser NLP tool utilizes various NLP techniques for information extraction. The key methods used in this tool include:

- Preprocessing: Tokenization, stop word removal, and part-of-speech tagging.
- Named Entity Recognition (NER): Identifying entities such as names, organizations, skills, etc.
- Regular Expressions: Pattern matching for extracting specific information.
- Custom Rules: Additional rules and heuristics for specific data extraction.

The `resume_parser.py` script provides the implementation of these methods along with relevant comments and explanations.

## Results

The parsed information from the resumes will be stored as JSON files in the `output` directory. Each JSON file corresponds to a single resume and contains the extracted information in a structured format.

Feel free to modify the parsing logic, output format, or add further analysis based on your requirements.

## Contributing

Contributions to this project are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue on the GitHub repository. Additionally, you can fork the repository, make your changes, and submit a pull request for review.

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify
