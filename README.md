Project by Nanditha Nair
# H
## D

Describe data and what's interesting about this data

The data used in this project is available in this repository, named ['hiphopcandidate.csv'](). It was sourced from the [FiveThirtyEight Repository](https://github.com/fivethirtyeight). 
To get into a usable format, the album year column had to be reformatted. This column orginally contained only the release year of each album, but had a _GENERAL_ data type. Changing the data type of this column to _DATE_ incorrectly transformed the data. (For example, 2011 would be transformed into 03/07/1905). To fix this issue, I used the 'Text to Column' function to transform the values in the column to _TEXT_ format. Afterwards, I could change the format of the whole column to _DATE_ type which allowed me to create pivot tables easily in the following steps.


Data Viz 1
This areachart captures trends in sentiments over time in mentions of Donald Trump in hip hop lyrics. 

> It was created by making a pivot table. This pivot table had filter set to candidate, columns set to sentiment, rows set to album_release_date, and values set to Count of candidate. From here, I filtered the candidate section to display only results for mentions of Donald Trump, to get a pivot table displaying counts of positive, neutral, and negative mentions of Trump for each year. 
This data was then used to create the data visualisation shown above.



Data Viz 2


Describe your analysis. What did you find interesting? What does the data show? What types of pivot tables did you run on the data? 
