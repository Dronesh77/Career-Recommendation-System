# Career and Industry Suggestion System

This project suggests the best career domain and industry based on the user's work experience and skills. It leverages natural language processing (NLP) techniques to analyze user input and matches it with predefined career domains and industries.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Data](#data)
- [Functions](#functions)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Career and Industry Suggestion System helps users determine the most suitable career path and industry based on their work experience and skills. It uses NLTK for text tokenization and stopword removal, and analyzes the input text against a set of predefined career domains and industries.

## Requirements

- Python 3.6+
- Jupyter Notebook
- NLTK library

## Setup

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/career-industry-suggestion-system.git
    cd career-industry-suggestion-system
    ```

2. **Install the required Python libraries**:
    ```sh
    pip install nltk
    ```

3. **Download NLTK data files**:
    Run the following commands in a Python shell or Jupyter Notebook:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

4. **Create CSV files**:
    Create two CSV files named `career_domains.csv` and `industries.csv` in the same directory as your Jupyter Notebook.

    **career_domains.csv**:
    ```csv
    domain,keywords
    fintech,finance financial investment banking
    edtech,education learning teaching
    healthtech,healthcare medical health
    agritech,agriculture farming
    logitech,technology electronics hardware
    non-tech-enterprises,business management sales
    e-commerce,online retail commerce
    travel tech,travel tourism hospitality
    IT services,information technology software services
    product services,manufacturing production
    ```

    **industries.csv**:
    ```csv
    industry,keywords
    advertising & marketing,advertising marketing branding
    agriculture,farming agricultural
    chemicals & resources,chemical resource mining petroleum
    construction,construction building
    consumer goods & FMCG,consumer goods fast-moving consumer goods fmcg
    e-commerce,e-commerce online shopping
    economy & politics,economy politics government
    energy & environment,energy environment sustainability
    finance & insurance,finance insurance
    internet,internet online web
    life,celebrities personal lifestyle
    media,media entertainment news
    metals & electronics,metals electronics manufacturing
    real estate,real estate property housing
    retail & trade,retail trade merchandise
    services,services consulting
    society,society culture demographics
    sports & recreation,sports recreation fitness
    technology & telecommunications,technology telecommunications hardware software
    transportation & logistics,transportation logistics
    travel, tourism & hospitality,travel tourism hospitality
    ```

## Usage

1. **Open the Jupyter Notebook**:
    ```sh
    jupyter notebook
    ```

2. **Run the notebook cells**:
    - The notebook is organized into sections. Follow the prompts to input your work experience and skills.

3. **View suggestions**:
    - After running the notebook, the system will suggest the best career domain and industry based on the input provided.

## Data

The data for career domains and industries is stored in CSV files:

- **career_domains.csv**: Contains career domains and associated keywords.
- **industries.csv**: Contains industries and associated keywords.

## Functions

- **read_csv_to_dict(file_path)**: Reads a CSV file and converts it into a dictionary.
- **tokenize_and_filter(text)**: Tokenizes the input text and removes stopwords.
- **analyze_text(tokens, categories)**: Analyzes tokens to compute scores for each category based on keyword matches.
- **suggest_career_and_industry(user_text, work_exp, career_domains, industries)**: Suggests the best career domain and industry based on the user's input text and work experience.
- **main()**: Main function to execute the workflow.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
