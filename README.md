# JobDataExtractionAndAnalysis

## Overview

JobDataExtractionAndAnalysis is a comprehensive project that combines web scraping and exploratory data analysis (EDA) to extract and analyze job listings from the TimesJobs website. The project utilizes Python, BeautifulSoup, Selenium, and NumPy to automate data extraction and perform insightful analysis.

## Table of Contents

1. [Features](#features)
2. [Data Source](#data-source)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Project Structure](#project-structure)
6. [Legal and Ethical Considerations](#legal-and-ethical-considerations)
7. [Future Improvements](#future-improvements)
8. [Contact](#contact)
9. [Contributing](#contributing)
10. [License](#license)

## Features

- **Data Extraction:**
  - Automated scraping of job listings using Selenium and BeautifulSoup.
  - Extraction of key job details such as company names, experience, skills, locations, salaries, and job links.
  - Storage of extracted data in CSV files for further analysis.

- **Data Analysis:**
  - Cleaning and preparation of job data using Pandas.
  - Normalization of salary data and computation of average salary and experience.
  - Visualization of data through histograms, scatter plots, and pie charts.
  - Frequency analysis of skills, companies, and locations.
  - Detection and filtering of salary outliers using z-scores.

## Data Source

The job data is scraped using scripts in the `Job_Extractor_Scripts` directory.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/elbehwash0/JobDataExtractionAndAnalysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd JobDataExtractionAndAnalysis
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Data Extraction

1. Navigate to the `Job_Extractor_Scripts` directory:
   ```bash
   cd Job_Extractor_Scripts
   ```
2. Update the `CHROMEDRIVER_PATH` in `Selenium_scrapper.py` and `csv_path` in `csv_Handler.py` as needed.
3. Run the main script to start scraping:
   ```bash
   python Selenium_scrapper.py
   ```

### Data Analysis

1. Navigate to the `EDA_Notebooks` directory:
   ```bash
   cd EDA_Notebooks
   ```
2. Run the notebooks to perform data cleaning and analysis.

## Project Structure

```
JobDataExtractionAndAnalysis/
│
├── Data/
│   └── (CSV files)
│
├── EDA_Notebooks/
│   ├── eda_jobs.ipynb
│   ├── jobs_data_cleaning_and_preparation.ipynb
│   └── README.md
│
├── Job_Extractor_Scripts/
│   ├── beautifulsoup_utils.py
│   ├── csv_handler.py
│   ├── Selenium_scrapper.py
│   ├── README.md
│   └── requirements.txt
│
└── README.md
```

## Legal and Ethical Considerations

Ensure compliance with the TimesJobs website's Terms of Service. Use the scraper responsibly and avoid overwhelming the website with requests.

## Future Improvements

- Enhance error handling and logging.
- Implement asynchronous scraping for efficiency.
- Expand support to additional job listing websites.
- Integrate proxy and user-agent rotation.
- Introduce a configuration file for dynamic settings.
- Develop a simple GUI for user-friendly interaction.

## Contact

For questions, feedback, or collaboration opportunities, feel free to reach out:

- **Email:** [abdullah.mohamed.9511@gmail.com](mailto:abdullah.mohamed.9511@gmail.com)
- **LinkedIn:** [Abdallah Mohamed](https://www.linkedin.com/in/abdallah-mohamed-4a78122b9/)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
