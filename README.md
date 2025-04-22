# Case Study Analysis with LLMs

This project analyzes case studies from various companies using Large Language Models (LLMs) to extract insights and patterns. It includes web scraping capabilities to gather case study data and LLM-based analysis to process and categorize the information.

## Features

- Web scraping of case studies from multiple sources
- LLM-powered analysis of case study content


## Prerequisites

- Python 3.9 or higher
- OpenAI API key

## Installation

1. Clone this repository:
```bash
git clone [your-repository-url]
cd [repository-name]
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the root directory and add your OpenAI API key:
```
OPENAI_API_KEY=your_api_key_here
```

## Project Structure

- `data_scraping.ipynb`: Jupyter notebook for scraping case studies from various web pages
- `llm_analysis.ipynb`: Jupyter notebook for analyzing case studies using LLMs
- `data/`: Directory containing input and output data files
  - `case_studies_links.csv`: Input file with case study URLs
  - `case_studies_scraped.csv`: Generated file with scraped case study content

## Usage

1. **Data Collection**:
   - Run the `data_scraping.ipynb` notebook to scrape case studies from the URLs in `case_studies_links.csv`
   - The scraped data will be saved to `data/case_studies_scraped.csv`

2. **Analysis**:
   - Run the `llm_analysis.ipynb` notebook to analyze the scraped case studies
   - The notebook uses GPT-4 to process and categorize the case study content

## Notes

- The `.env` file is ignored by git to protect your API key
- Generated data files are also ignored to keep the repository clean
- Make sure to keep your API key secure and never commit it to the repository 