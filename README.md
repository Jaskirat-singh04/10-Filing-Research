# SEC 10-K Filings Analysis

This project aims to analyze the 10-K filings of a company (in this case, Microsoft) to extract insights related to revenue, debt, and management perspectives. Additionally, it calculates a risk score based on these factors for each year and visualizes the risk scores over time.

## Demo Video is in Description.

## Tech Stack

### Python
Python is a widely-used, interpreted, high-level programming language known for its simplicity, readability, and extensive ecosystem of libraries. It was chosen for this project due to its ease of use and powerful data manipulation and visualization capabilities.

### SEC-Edgar-Downloader
The `sec-edgar-downloader` library is a Python package that facilitates downloading SEC filings, such as 10-K reports, from the EDGAR database. This library was chosen for its convenience and direct integration with the SEC's EDGAR system.

### Google Generative AI (Gemini-Pro)
The Google Generative AI (Gemini-Pro) model is a large language model (LLM) used for generating textual insights from the 10-K filings. This LLM was chosen because it is free, relatively fast, and provides good results for the task at hand.

### Regular Expressions (re)
The built-in `re` module in Python is used for pattern matching and text manipulation. Regular expressions are employed to extract relevant information from the generated insights, such as revenue, debt, and risk scores.

### Pandas
Pandas is a powerful data manipulation and analysis library for Python. It is used in this project to read and process the extracted data from the CSV file and prepare it for visualization.

### Matplotlib
Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. It is utilized in this project to create a line graph that visualizes the risk scores over time.

### Streamlit
Streamlit provides fast frontend development for AI/ML projects.

## Project Structure

The project consists of the following main components:

1. **Data Downloading**: The `sec-edgar-downloader` library is used to download the 10-K filings for Microsoft from the SEC's EDGAR database.
2. **Text Cleaning**: The downloaded filings are cleaned using regular expressions and other text processing techniques to remove HTML tags, special characters, and noise.
3. **Insight Generation**: The cleaned text is split into smaller sections, and the Gemini-Pro LLM is used to generate insights for each section, focusing on revenue, debt, and management perspectives.
4. **Data Formatting**: The generated insights are cleaned and formatted into a consistent structure using the Gemini-Pro LLM and regular expressions.
5. **Risk Score Extraction**: Regular expressions are employed to extract the risk scores from the formatted data for each year.
6. **Data Visualization**: The risk scores are saved to a CSV file, and the Pandas library is used to read and process the data. Finally, Matplotlib is utilized to create a line graph visualizing the risk scores over time.

## Usage

1. Clone the repository or download the source code.
2. Install the required dependencies by running `pip install sec-edgar-downloader google-generativeai pandas matplotlib`.
3. Set up the Google Generative AI API key in the provided code.
4. Run the code to download the 10-K filings, generate insights, extract risk scores, and visualize the data.

Note: The project assumes the presence of the `sec-edgar-filings/MSFT` directory containing the downloaded 10-K filings for Microsoft. If this directory is not present, the code will attempt to download the filings automatically.

## Contributing

Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.
