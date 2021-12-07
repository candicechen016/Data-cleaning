# Data Cleaning Final Project   
 
This is a group project of the IS 537 data cleaning course in Fall 2021 at UIUC. 


## Project Description
  
*Starbucks now operates more than 28,289 retail stores in 49 countries. This dataset includes a record for every Starbucks or subsidiary store location currently in operation as of Nov 2021.*

**Dataset source:**  
https://www.kaggle.com/kukuroo3/starbucks-locations-worldwide-2021-version 

**Pre-processing:**
* Download the dataset and sort rows by country names. 
* Choose The Group of Seven (G7) as our analysis subjects, which are the United States, Canada, France, Germany, Italy, and Japan. 
* Remove the rest of countries and add a new column as index considering for better separating work to members, and for convenience to avoid the wrong sequence at the time combining again. 
* The output for our members to process is startbucks_new2.csv.

**We tried to analyze these topics from the dataset:**
1. What are the average opening hours in major cities?
2. Would different ownership types influence opening hours?
3. What are the closed days for branches in the same time zone?

**Major cleaning tasks:**
1. Filter countries into a subset. 
2. Split the **_schedule_** column into 7 days then fill in opening and closed hours as values.
3. Processing uppercase and lowercase strings in the **_city_** and the **_countrySubdivisionCode_** column.   
4. Split the **_olsonTimeZoneId_** column into GMT and its region.
5. Merge three columns regarding the address. Since there are variations between different countries in the way of filling correct format to three address columns, we think it's better to present in only one column with complete information instead of fragmented words.
6. Standardize the **_city_** column based on each country's format.
7. Drop unrelated columns.

**Teamwork:**
* Each member proposed some datasets then we chose one of them as our subject after discussion.
* Briefly checked the dataset by columns. Meanwhile, everyone came up with some questions that lead to what information we need to analyze and how to get them from this dataset.
* Created subset of the dataset by countries and each member took one of them to clean with their preferred tools.
* _starbucks_final_tidy.csv_ is the final tidy version dataset combined with all members' subsets

**My part:**
* This Notebook contains Japan and part of the US. We combined cleaned parts in another tool.
* Used Python as a major cleaning tool. Used Excel for the final step of correcting some typos in Japanese city names.
* More detailed processing steps documented in the Jupyter notebook file, cleaning_process.ipynb.
* My tidy version is _startbucks_jp_us2132_cleaned.csv_.

