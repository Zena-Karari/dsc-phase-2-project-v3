# Analyzing Top-Performing Films for Strategic Success

## Overview
This project supports a 5-year corporate strategy for a company launching its own movie studio to create original video content. With no prior film production experience, the company aims to use data-driven insights to understand box office trends and guide its investment decisions. The analysis focuses on film performance across genres, individual movies, production budgets, and ratings to maximize commercial success and return on investment (ROI).

### Repository Contents
- **`student.ipynb`** - Jupyter notebook with detailed data exploration, analysis, visualizations, and statistical tests.
- **`presentation.pdf`** - Summary of key findings and recommendations.
- **Data Files** - From Box Office Mojo, IMDb, Rotten Tomatoes, The Movie DB, and The Numbers.

## Objectives
- Identify the top 10 best-performing genres based on ROI and worldwide gross sales.
- Identify the top 10 best-performing movies based on ROI and worldwide gross sales.
- Examine the relationship between production costs and global film sales.
- Assess the impact of movie ratings on global film sales.

## Group Members
- Evan Ndungu
- Viola Kimitei
- Robert Sumaili
- Zeena Lisa Karari

## Setup Instructions
### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or VS Code with Jupyter extension
- SQLite3 (for database access)
- Required Python libraries (listed below)

### Installation
#### Clone the Repository
bash
git clone <repository-url>
cd group4_phase2_project

#### Install Dependencies
bash
pip install pandas numpy plotly matplotlib seaborn statsmodels sqlite3

#### Verify Data Files
Ensure all data files are in the `data/` directory as listed above. The notebook expects:
- `im.db`: SQLite database with `movie_basics` and `movie_ratings` tables.
- `rt.movie_info.tsv` and `rt_reviews.tsv`: Tab-delimited Rotten Tomatoes files.
- `movie_budget.csv`: Budget and gross data (adjust file name/path if different).

#### Run the Notebook
Open the notebook in Jupyter or VS Code:
```bash
jupyter notebook student.ipynb
```
Or in VS Code:
1. Open `student.ipynb`.
2. Run all cells.



## Data Sources
- **Box Office Mojo**: Budget and gross data ([boxofficemojo.com](https://www.boxofficemojo.com))
- **IMDb**: Movie basics and ratings ([imdb.com](https://www.imdb.com))
- **Rotten Tomatoes**: Movie info and reviews ([rottentomatoes.com](https://www.rottentomatoes.com))
- **The Movie DB**: Additional movie details ([themoviedb.org](https://www.themoviedb.org))
- **The Numbers**: Financial data ([the-numbers.com](https://www.the-numbers.com))

## Key Findings

### Top-Performing Genres
#### By ROI:
1. Biography, Documentary (5261.66%)
2. Drama, Family, Fantasy (4726.02%)
3. Crime, Drama, Family (3352.97%)

_All top 10 genres exceed 1000% ROI, led by Biography, Documentary._

#### By Sales:
1. Adventure, Drama, Sport ($1.27B)
2. Fantasy, Romance ($1.27B)
3. Family, Fantasy, Musical ($933M)

_Action and adventure genres dominate high-grossing films._

### Top-Performing Movies
#### By Sales:
1. Avatar ($2.78B)
2. Titanic ($2.21B)
3. Avengers: Infinity War ($2.05B)

#### By ROI:
1. The Gallows (41556.47%)
2. Bambi (31135.43%)
3. Rocky (22400.00%)

_High-sales movies differ from high-ROI movies, showing profitability doesn’t always align with revenue._

### Relationships
- **Production Budget vs. Sales:** Strong correlation (R² = 0.605), with budgets influencing up to 60.5% of global sales.
- **Ratings vs. Sales:** Weak positive correlation (R² = 0.027), with ratings impacting sales by ~2.7%.

_Higher-rated films tend to be more profitable, but budget has a greater effect on revenue._

### Market Trends
- Superhero films (e.g., Avatar) lead in global sales.
- Family-friendly animated films (e.g., Biography, Documentary) excel in ROI.
- Higher budgets often yield higher revenue, but not always better ROI.

## Recommendations
1. **Genre Focus:** Invest in Biography, Documentary, Drama, Family, Fantasy, and Action/Adventure genres for high ROI and sales potential.
2. **Production Investment:** Increase production budgets to maximize sales (up to 60.5% impact).
3. **Quality Focus:** Produce high-quality films to achieve better ratings, boosting sales by up to 2.7%.

## Conclusion
For a profitable studio launch, the company should prioritize high-ROI genres like Biography and Documentary while strategically increasing production budgets to drive sales. Quality films with strong ratings will further enhance market performance, aligning with current trends and audience preferences.




