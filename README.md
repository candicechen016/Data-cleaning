# Data Cleaning Final Project   
 
This is a group project of the IS 537 data cleaning course in Fall 2021 at UIUC. 

  
**Dataset source:**  
https://www.kaggle.com/kukuroo3/starbucks-locations-worldwide-2021-version 
  
Starbucks now operates more than 28,289 retail stores in 49 countries. This dataset includes a record for every Starbucks or subsidiary store location currently in operation as of Nov 2021.  

**We tried to analyzed these topics from this dataset:**
1. What is the average opening hours in major cities?
2. Ownership type differences?
3. What is the closed days for branches in the same time zone?

**Major cleaning tasks:**
1. Filter countries into subset. We choose The Group of Seven (G7) as our anlyze subjects, which are United States, Canada, France, Germany, Italy, and Japan.
2. Split the "schedule" column into 7 days then fill in opening and closed hours as values.
3. Processing uppercase and lowercase strings in "city" and "countrySubdivisionCode" column.   
4. Split the "olsonTimeZoneId" column into GMT and its region.
5. Merge three columns regarding address. Since there are varions between different countries in the way filling correct format to three address columns, we think it's better to present in only one column with complete information instead of fragmented words.
6. Standardize 'City' column based on each country's format.
7. Drop unrelated columns.

**Teamwork:**
* Each member propose some datasets then we chose one of them as our subject after discussion.
* Briefly checked the dataset by columns. Meanwhile, everyone came up some questions that lead to what information we need to analyze and how to get them from this dataset.
* Created subset of the dataset by countries and each member took one of them to clean with their preferreble tools.

**My part:**
* This Notebook contains Japan and part of US. We combined cleaned parts in another tool.
* Uesd Python as major cleaning tool. Used Excel for the final step of correcting some typos in Japanese city names.

**More detailed processing steps documented in the Jupyter notebook file, IS537 Data Cleaning Final Project.ipynb.**
