# Overview
This project involves cleaning and preprocessing a Netflix movies and TV shows dataset to prepare it for analysis. The original dataset contained information about Netflix titles with various attributes like title, director, cast, country, release year, rating, duration, and more.

# Cleaning Steps Performed
1. *Missing Values Analysis*:
   - Identified missing values in director , cast, country, and date_added.
   - Maintained as-is since these represent legitimate missing data

2. *Text Cleaning*:
   - Removed leading/trailing spaces from all text fields
   - Fixed malformed special characters (dashes and apostrophes)
   - Standardized country names to use only the first listed country

3. *Date Standardization*:
   - Converted date_added to datetime format
   - One invalid date record was set to NaT

4. *Duration Column Processing*:
   - Split into numeric duration and unit (minutes or seasons)
   - Created two new columns: duration_num and duration_unit

5. *Data Type Conversion*:
   - Ensured proper data types for all columns
   - Created separate numeric duration column for analysis

6. *Duplicate Check*:
   - Verified no complete duplicate rows existed
