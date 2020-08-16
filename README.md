Project by Nanditha Nair
# H
## D

Describe data and what's interesting about this data

The data used in this project is available in this repository, named ['hiphopcandidate.csv'](). It was sourced from the [FiveThirtyEight Repository](https://github.com/fivethirtyeight). 
To get into a usable format, the album year column had to be reformatted. This column orginally contained only the release year of each album, but had a _GENERAL_ data type. Changing the data type of this column to _DATE_ incorrectly transformed the data. (For example, 2011 would be transformed into 03/07/1905). To fix this issue, I used the 'Text to Column' function to transform the values in the column to _TEXT_ format. Afterwards, I could change the format of the whole column to _DATE_ type which allowed me to create pivot tables easily in the following steps.


Data Visualisation 1:
This stacked bar chart captures trends in sentiments over time in mentions of Donald Trump in hip hop lyrics. 

![alt text](dataviz1.png)

> It was created by making a pivot table. This pivot table had filter set to candidate, columns set to sentiment, rows set to album_release_date, and values set to Count of candidate. From here, I filtered the candidate section to display only results for mentions of Donald Trump, to get a pivot table displaying counts of positive, neutral, and negative mentions of Trump for each year. 
This data was then used to create the data visualisation shown above.

### Analysis:
The data visualisation shows that the number of times Trump has been mentioned in hiphop lyrics have generally increased, from only 3 total mentions in 1989 and to a peak of 33 mentions in 2013. It also shows that while his general popularity in song lyrics has generally increased, sentiments towards him have soured over time. Mentions of Trump from late 80s to the early 2000s were almost exclusively positive or neutral. However, in 2015 there was an explosion in the number of mentions of Trump with negative sentiments, and by 2016 negative mentions of Trump were almost 4 times more common as positive ones. This is no doubt a reflection of changes in how the media in general has portrayed Trump. In the late 80s and early 2000s Trump was mostly seen an image of wealth, with his name popping up on lists like "Ten most admired men and women living of 2011". However since launching his presidential campaign in 2015, he has received more scrutiny for his views which correlates with the rise in negative sentiments towards him in hip hop. 


Data Viz 2


Describe your analysis. What did you find interesting? What does the data show? What types of pivot tables did you run on the data? 
