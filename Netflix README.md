# Netflix / OTT Content Analysis

Exploratory data analysis of 8,800+ Netflix titles to understand genre popularity,
release trends, and the Movies vs. TV Shows split.

## Dataset
[Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows) (Kaggle)

## What I did
- Cleaned raw data: handled missing values in `director`, `cast`, and `country`;
  parsed `date_added` into proper datetime format; split multi-valued genre
  strings (`listed_in`) into individual genres.
- Analyzed the Movies vs. TV Shows split.
- Identified the most common genres by title count.
- Tracked how content additions changed year over year.
- Identified the top content-producing countries.

## Tools
Python, Pandas, Matplotlib, Seaborn (in Google Colab)

## Files
- `netflix_analysis.ipynb` — full cleaning + analysis notebook
- `movies_vs_tvshows.png` — Movies vs TV Shows chart
- `top_genres.png` — Top 10 genres chart
- `titles_per_year.png` — Titles added per year chart

## Key Findings
1. **Content mix:** 69.7% of titles are Movies (6,129) vs. 30.3% TV Shows (2,664).
2. **Top genres:** International Movies (2,752), Dramas (2,426), Comedies (1,674),
   International TV Shows (1,349), and Documentaries (869) are the most common
   categories.
3. **Growth trend:** Titles added per year grew sharply from 428 in 2016 to a
   peak of 2,016 in 2019, then declined to 1,498 by 2021 (the dataset's
   coverage ends mid-2021, which explains the drop-off).
4. **Top content-producing countries:** United States (2,812), India (972),
   United Kingdom (418), Japan (243), and South Korea (199) lead in title count.

## How to run
Open `netflix_analysis.ipynb` in Google Colab or Jupyter, upload
`netflix_titles.csv` from the Kaggle link above, and run all cells in order.
