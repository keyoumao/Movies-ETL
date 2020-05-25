# Movies-ETL

## Methods

Please refer to the challenge.py (https://github.com/keyoumao/Movies-ETL/blob/master/challenge.py) module for the transformation-data function for cletransform(Wikipediadata, Kagglemetadata, MovieLensratingdata):

- General function to load all three data files:
    Wikipedia data
    Kaggle metadata
    MovieLens rating data (from Kaggle)
- Multiple functions perform all of the transformation steps.
- Remove the existing data from SQL, but keep the empty tables and then load dataframe into PostgreSQL.
- **try-except** blocks were used account for unforeseen problems that may arise with new data.

## Assumptions

1. Kaggle database is superior to the Wikipedia jason data files.
2. Wikipedia data could fill in some of the missing values from Kaggle data files such as "runtime", "budget" and "revenue".
3. We take the "adult" as FALSE.
4. The *The Million Dollar Hotel* is the "best movie" with most 5.0 ratings.
5. The *Syriana* is the "worst" movie with most 0.5 ratings.
6. Run time only include the units of hours, hours-minutes, or minutes.
