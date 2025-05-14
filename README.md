# What-Drives-Anime-Scores

## Introduction, Data Selection & Motivation  
Anime studios produce dozens of series each season—but which factors drive high audience ratings? In this project, I explore a Kaggle anime metadata dataset to identify the combination of genres, themes, target demographics, and production features most strongly associated with weighted scores. As an avid TV enthusiast, I’m passionate about uncovering the patterns that make certain shows resonate. My goal is to give production houses a data-driven framework for greenlighting projects that mazimize viewer engagement. 

## Methodology  
1. **Data Cleaning & Feature Engineering**  
   - Filtered out entries with missing scores or metadata  
   - Created dummy variables for multi-label columns (genres, themes)  
   - Encoded demographic, type, and studio reputation as categorical features  
2. **Exploratory Data Analysis**  
   - Visualized score distributions by genre and demographic  
   - Tested correlations to pinpoint candidate predictors  
3. **Multiple Regression Modeling**  
   - Fitted an OLS model using `statsmodels`  
   - Evaluated R², p-values, and multicollinearity   
   - Refined by removing non-significant variables to isolate key drivers  
4. **Interpretation & Recommendations**  
   - Ranked the top coefficients to derive actionable insights  

## Project Structure 

├ README.md
├── code/
│ └── analysis.py ← script version of the notebook
├── data/
│ └── top_anime_dataset_v2.csv ← original raw dataset
└── docs/
├── project_paper.pdf ← detailed project report
└── slide_deck.pdf ← summary presentation slides

## Usage
  
1.  **Clone the repository**  
   ```bash
   git clone https://github.com/shanayamehra/What-Drives-Anime-Scores.git
   cd What-Drives-Anime-Scores

2. **Install dependencies**
    pip install pandas numpy statsmodels matplotlib jupyter

3. **Run the script**
   python code/analysis.py

## Conclusion

This regression study reveals that a mix of action/fantasy genres, shōnen demographic targeting, mid-length series formats (24–26 episodes), and renowned studios have the strongest positive impact on weighted scores. By prioritizing these characteristics, production teams can better allocate resources and greenlight projects with higher expected audience approval.
