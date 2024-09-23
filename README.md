Project Title
This repository contains the code, data, and results for our sentiment analysis of political speeches, with a focus on comparing rhetoric between presidential debates and rallies.

Contents of the Repository
README.md: This file, providing an overview of the project structure, tools, and steps for reproducing results.
LICENSE.md: Contains the license for the project (MIT License).
SCRIPTS: Folder containing all the Python scripts used for data preprocessing, sentiment analysis, and result generation.
DATA: Folder containing the raw and processed data used in the analysis.
OUTPUT: Folder containing the results of the analysis, including CSV files and visualizations.
Software and Platform
Software
Python 3.8 or higher
Required Packages
pandas
numpy
re (built-in)
csv (built-in)
vaderSentiment (for sentiment analysis)
matplotlib (for plots)
seaborn (for enhanced plotting)
Platform
The project has been tested on:

Windows 10/11
macOS
Linux (Ubuntu 20.04 and above)
Map of the Repository Structure
graphql
Copy code
/Project-Repository
│
├── README.md            # Orientation document
├── LICENSE.md           # MIT License for the repository
├── SCRIPTS/             # Python scripts for analysis
│   ├── data_preprocessing.py   # Script for cleaning and preparing data
│   ├── sentiment_analysis.py   # Script for performing sentiment analysis
│   └── generate_plots.py       # Script for creating visualizations
│
├── DATA/                # Folder for data storage
│   ├── raw/             # Raw data
│   └── processed/       # Processed data used in the analysis
│
├── OUTPUT/              # Results and output files
│   ├── csv/             # CSVs generated from analysis
│   └── visualizations/  # Plots and graphs generated from the data
Instructions for Reproducing Results
Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/project.git
cd project
Install the required packages: You can use pip to install the required packages:

bash
Copy code
pip install pandas numpy vaderSentiment matplotlib seaborn
Prepare the data: Ensure the raw data files are placed in the /DATA/raw/ folder. Run the preprocessing script to clean and structure the data:

bash
Copy code
python SCRIPTS/data_preprocessing.py
Perform sentiment analysis: After the data is processed, run the sentiment analysis script:

bash
Copy code
python SCRIPTS/sentiment_analysis.py
Generate visualizations: To create the plots from the analysis, run the following script:

bash
Copy code
python SCRIPTS/generate_plots.py
Check the results: All results, including CSV files and visualizations, will be stored in the /OUTPUT/ folder. The key output files include sentiment scores, comparison tables, and visualizations highlighting the sentiment differences between candidates at rallies and debates.
