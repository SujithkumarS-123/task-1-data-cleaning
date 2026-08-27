#Task 1: Data Cleaning and Preprocessing

## Objective

Clean and prepare a raw dataset with missing values, duplicate checks, inconsistent formats, and data-type validation using Python and Pandas.

## Dataset

Netflix Movies and TV Shows dataset.

## Tools Used

- Python
- Pandas
- Google Colab
- GitHub

## Data Cleaning Steps

1. Loaded the raw Netflix dataset into Pandas.
2. Checked the dataset structure, columns, data types, missing values, and duplicate rows.
3. Cleaned the column headers by converting them to lowercase and replacing spaces with underscores.
4. Filled missing values:
   - `director`, `cast`, and `country` were filled with `Not Available`.
   - `rating` was filled with `Not Rated`.
   - Missing `date_added` values were labelled as `Not Available`.
5. Removed duplicate rows using `drop_duplicates()`.
6. Removed leading and trailing spaces from text columns.
7. Standardized selected text fields:
   - `type` was standardized using title case.
   - `country` was standardized using title case.
   - `rating` was standardized using uppercase.
8. Converted `date_added` to datetime during preprocessing and formatted valid dates consistently as `dd-mm-yyyy`.
9. Converted `release_year` to an integer numeric data type.
10. Performed final checks for missing values, duplicates, and data types.
11. Exported the cleaned data as `cleaned_netflix_titles.csv`.

## Files

- `netflix_titles.csv` — Original raw dataset
- `netflix_cleaned_final.csv` — Cleaned dataset
- `Task_1_Data_Cleaning.ipynb` — Python/Pandas data-cleaning process in Google Colab

## Outcome

The dataset was cleaned and prepared for future analysis. It has consistent column headers, standardized text fields, a consistent date format, corrected data types, no missing values, and no duplicate rows.
