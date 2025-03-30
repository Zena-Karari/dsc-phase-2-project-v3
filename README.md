# Group 4 Phase 2 Project: Analyzing Top-Performing Films for Strategic Success

## Project Title
**Analyzing Top-Performing Films for Strategic Success**

## Overview
This project supports a 5-year corporate strategy for a company launching its own movie studio to create original video content. With no prior film production experience, the company aims to use data-driven insights to understand box office trends and guide its investment decisions. The analysis focuses on film performance across genres, individual movies, production budgets, and ratings to maximize commercial success and return on investment (ROI).

The repository includes:
1. A Jupyter notebook (`film_analysis.ipynb`) with detailed data exploration, analysis, visualizations, and statistical tests.
2. A presentation (`presentation.pdf`) summarizing key findings and recommendations.
3. Supporting data files from Box Office Mojo, IMDb, Rotten Tomatoes, The Movie DB, and The Numbers.

### Objectives
- Identify the top 10 best-performing genres based on ROI and worldwide gross sales.
- Identify the top 10 best-performing movies based on ROI and worldwide gross sales.
- Examine the relationship between production costs and global film sales.
- Assess the impact of movie ratings on global film sales.

### Group Members
- Evan Ndungu
- Viola Kimitei
- Robert Sumaili
- Zeena Lisa Karari

## Project Structure
group4_phase2_project/
├── data/
│   ├── im.db              # SQLite database with IMDb data
│   ├── rt.movie_info.tsv  # Rotten Tomatoes movie info (tab-delimited)
│   ├── rt_reviews.tsv     # Rotten Tomatoes reviews (tab-delimited)
│   ├── movie_budget.csv   # Budget and gross data (assumed format)
│   └── ...                # Additional data files as needed
├── film_analysis.ipynb    # Jupyter notebook with full analysis
├── presentation.pdf       # Summary presentation slides
└── README.md              # This file

## Setup Instructions
To run the analysis locally, follow these steps:

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or VS Code with Jupyter extension
- SQLite3 (for database access)
- Required Python libraries (listed below)

### Installation
 **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd group4_phase2_project
Install Dependencies Install the required Python libraries using pip:
bash

Collapse

Wrap

Copy
pip install pandas numpy plotly matplotlib seaborn statsmodels sqlite3
Verify Data Files Ensure all data files are in the data/ directory as listed above. The notebook expects:
im.db: SQLite database with movie_basics and movie_ratings tables.
rt.movie_info.tsv and rt_reviews.tsv: Tab-delimited Rotten Tomatoes files.
movie_budget.csv: Budget and gross data (adjust file name/path if different).
Run the Notebook Open the notebook in Jupyter or VS Code:
bash

Collapse

Wrap

Copy
jupyter notebook film_analysis.ipynb
Or in VS Code, open film_analysis.ipynb and run all cells.
Saving as PDF
To save the notebook with outputs as a PDF:

In VS Code:
Open film_analysis.ipynb.
Click "..." on the toolbar, select "Export," and choose "HTML."
Open the HTML file in a browser, then print to PDF (File > Print > Save as PDF).
Command Line (requires LaTeX):
bash

Collapse

Wrap

Copy
jupyter nbconvert --to pdf film_analysis.ipynb
Data Sources
Box Office Mojo: Budget and gross data (boxofficemojo.com)
IMDb: Movie basics and ratings (imdb.com)
Rotten Tomatoes: Movie info and reviews (rottentomatoes.com)
The Movie DB: Additional movie details (themoviedb.org)
The Numbers: Financial data (the-numbers.com)
Key Findings
Top-Performing Genres
By ROI:
Biography, Documentary (5261.66%)
Drama, Family, Fantasy (4726.02%)
Crime, Drama, Family (3352.97%)
All top 10 genres exceed 1000% ROI, led by Biography, Documentary.
By Sales:
Adventure, Drama, Sport ($1.27B)
Fantasy, Romance ($1.27B)
Family, Fantasy, Musical ($933M)
Action and adventure genres dominate high-grossing films.
Top-Performing Movies
By Sales:
Avatar ($2.78B)
Titanic ($2.21B)
Avengers: Infinity War ($2.05B)
By ROI:
The Gallows (41556.47%)
Bambi (31135.43%)
Rocky (22400.00%)
High-sales movies differ from high-ROI movies, showing profitability doesn’t always align with revenue.
Relationships
Production Budget vs. Sales: Strong correlation (R² = 0.605), with budgets influencing up to 60.5% of global sales.
Ratings vs. Sales: Weak positive correlation (R² = 0.027), with ratings impacting sales by ~2.7%.
Higher-rated films tend to be more profitable, but budget has a greater effect on revenue.
Market Trends
Superhero films (e.g., Avatar) lead in global sales.
Family-friendly animated films (e.g., Biography, Documentary) excel in ROI.
Higher budgets often yield higher revenue, but not always better ROI.
Recommendations
Genre Focus: Invest in Biography, Documentary, Drama, Family, Fantasy, and Action/Adventure genres for high ROI and sales potential.
Production Investment: Increase production budgets to maximize sales (up to 60.5% impact).
Quality Focus: Produce high-quality films to achieve better ratings, boosting sales by up to 2.7%.
Conclusion
For a profitable studio launch, the company should prioritize high-ROI genres like Biography, Documentary, while strategically increasing production budgets to drive sales. Quality films with strong ratings will further enhance market performance, aligning with current trends and audience preferences.

Notes
The notebook includes bar charts, histograms, scatter plots, and regression analyses to support findings.
OCR errors (e.g., "gmovies" instead of "movies") were corrected in this README.
Ensure data files match the notebook’s expected format to avoid runtime errors.
text

Collapse

Wrap

Copy

---

### Saving the File
To use this as a `.md` file:
1. Copy the content above (excluding the outer ```markdown markers).
2. Paste it into a text editor (e.g., VS Code, Notepad).
3. Save it as `README.md` in your project directory.

This file will render properly in Markd