# Presidential Candidate Sentiment Analysis

This repository contains the code, data, and results for our sentiment analysis of political speeches, with a focus on comparing rhetoric between presidential debates and rallies.

## Contents of the Repository

- **README.md**: This file, providing an overview of the project structure, tools, and steps for reproducing results.
- **LICENSE.md**: Contains the license for the project (MIT License).
- **SCRIPTS**: Folder containing all the Python scripts used for data preprocessing, exploratory data analysis, sentiment analysis, and result visualization.
- **DATA**: Folder containing the raw and processed data used in the analysis.
- **OUTPUT**: Folder containing the results of the analysis, including CSV files and visualizations.

## Software and Platform

### Software
- Python 3.8 or higher

### Required Packages
- pandas
- numpy
- re (built-in)
- csv (built-in)
- vaderSentiment (for sentiment analysis)
- matplotlib (for plots)
- seaborn (for enhanced plotting)



### Platform
The project has been tested on:
- macOS

## Map of the Repository Structure

```plaintext
/Project-Repository
│
├── README.md            # Orientation document
├── LICENSE.md           # MIT License for the repository
├── SCRIPTS/             # Python scripts for analysis
│   ├── Data_Preprocess.ipynb      # Script for cleaning and preparing data
│   ├── Sentiment_Analysis.ipynb   # Script for performing sentiment analysis
│   ├── Visualitationzs.ipynb      # Script for creating visualizations
│   └── eda.ipynb                  # Script for exploratory data analysis
│
├── DATA/                # Folder for data storage
│   ├── raw/             # Raw data
│      ├── Debate_Transcript.txt                # Transcript of all speech at presidential debate
│      ├── Harris_Philadelphia_Transcript.txt   # Transcript of Harris's Philadelphia rally 
│      ├── Trump_Wisconsin_Transcript.txt       # Transcript of Trump's Wisconsin rally
│   └── processed/       # Processed data used in the analysis
│      ├── Processed_Transcripts_Data.csv       # csv with all speech entries and categorical Speaker and Topic data
│      ├── Scored_Data.csv                      # same as Processed_Transcripts_Data but including sentiment scores
│
├── OUTPUT/              # Results and output files
│   ├── csv/             # CSVs generated from analysis
│   └── visualizations/  # Plots and graphs generated from the data
│      ├── avg_sentiment_debate.png    # sentiment scores from the debate grouped by Speaker and Topic
│      ├── avg_sentiment_rally.png     # sentiment scores from the rallies grouped by Speaker and Topic
│      ├── score_harris_debate.png     # histogram distribution of Harris's debate speech
│      ├── score_harris_rally.png      # histogram distribution of Harris's rally speech
│      ├── score_trump_debate.png      # histogram distribution of Trump's debate speech
│      ├── score_trump_rally.png       # histogram distribution of Trump's rally speech
│      ├── violin_plot.png             # violin plots contrasting each candidate's speech distribution at their rallies and at the debate
```
## Instructions for Reproducing Results

1. **Clone the repository**:
   ```bash
   git clone https://github.com/bwillow1222/ds4003MI3P1.git
   cd project
2. **Install the required packages**
   ```bash
   pip install pandas numpy vaderSentiment matplotlib seaborn
3. **Prepare the data**
   ```bash
   python SCRIPTS/Data_Preprocess.ipynb
4. **Perform sentiment analysis**
   ```bash
   python SCRIPTS/Sentiment_Analysis.ipynb
5. **Generate visualizations**
   ```bash
   python SCRIPTS/Visualitationzs.ipynb
6. **Check the results:**
   All results, including CSV files and visualizations, will be stored in the /OUTPUT/ folder. The key output files include sentiment scores, comparison tables, and visualizations highlighting the sentiment differences between candidates at rallies and debates.
