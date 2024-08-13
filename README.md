 # CSV Data Extractor App
This project is a WPF (Windows Presentation Foundation) application designed to process stock market transaction data from multiple banks, each providing data in CSV format with different schemas. The application extracts specified fields, including both simple and complex data fields, from the input files and generates a standardized CSV output.
## Features
*	**User-Friendly Interface:** A simple and intuitive WPF application that allows users to process CSV files with ease.
  
*	**Simple Field Extraction:** Extracts configurable simple fields (e.g., ISIN, CFICode, Venue) directly from the CSV file.
  
*	**Complex Field Parsing:** Parses complex fields (e.g., AlgoParams) to extract specific values (e.g., PriceMultiplier) and outputs them under standardized headers (e.g., Contract Size).
  
*	**Automatic Output Generation:** The application generates an output CSV file in the same location as the input file with the name [inputfilename].extracted.csv.
  
## How It Works
**1.	Input Parameters:**
*	**Bank Name:** Select the bank whose CSV schema is being processed.
*	**Input CSV File:** Browse and select the CSV file containing the stock market transaction data.
  
**2.	Processing:**
*	Once the inputs are provided, click the "Process" button.
*	The application will process the input file according to the specified configurations and generate the output file.

**3.	Output:**
*	The output file is saved in the same directory as the input file with the name **[inputfilename].extracted.csv**.
## Usage
1.	Run the application.
2.	Provide the required inputs (bank name and input CSV file).
3.	Click on the "Process" button.
4.	The output file will be generated and saved in the same location as the input file.
   
## Project Structure
*	**CsvProcessor:** Contains the core logic for processing CSV files, including field extraction and parsing.
  
*	**DataExtractor:** The WPF application with the user interface for interacting with the CSV processing logic.
  
*	**LoggerUtility:** Contains the logic for logging information and errors.
  
*	**DataExtractor.NUnit:** Unit tests to ensure the reliability of the CSV processing logic.

## Getting Started
Clone the repository, open the solution in Visual Studio, and build the project. Run the application to start processing CSV files.
