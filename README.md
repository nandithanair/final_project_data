# Hip Hop Lyric Mentions of 2016 US Primary Candidates
Project by Nanditha Nair

This dataset shows the number of mentions of 2016 US primary candidates in hip hop songs. It includes not only the number of mentions for each candidate for every year from 1989 to 2016, but also the sentiment towards the candidate in each mention (either positive, neutral, or negative) as well as the theme of the mention. This dataset is fascinating because it can be used to display evolving sentiments towards candidates in the hip hop scene.

## Dataset Source and Data Cleaning / Formatting:
The data used in this project is available in this repository, named ['hiphopcandidate.csv'](https://raw.githubusercontent.com/fivethirtyeight/data/master/hip-hop-candidate-lyrics/genius_hip_hop_lyrics.csv). It was sourced from the [FiveThirtyEight Repository](https://github.com/fivethirtyeight). FiveThirtyEight has published its [own analysis of this dataset](https://projects.fivethirtyeight.com/clinton-trump-hip-hop-lyrics/), which varies from this one in its area of focus. 

To get the dataset into a usable format, the album year column had to be reformatted. This column orginally contained only the release year of each album, but had a _GENERAL_ data type. Changing the data type of this column to _DATE_ incorrectly transformed the data. (For example, 2011 would be transformed into 03/07/1905). To fix this issue, I used the 'Text to Column' function to transform the values in the column to _TEXT_ format. Afterwards, I could change the format of the whole column to _DATE_ type which allowed me to create pivot tables easily in the following steps.


## Change in Sentiments Towards Trump:
This stacked bar chart captures trends in sentiments over time in mentions of Donald Trump in hip hop lyrics. 

![Changes in Sentiments Towards Trump in Hip Hop Lyric Mentions](https://media.journalism.berkeley.edu/upload/2020/08/15976090096304582.png)

> This chart was created through the use of a pivot table. The pivot table had _filter_ set to 'candidate', _columns_ set to 'sentiment', _rows_ set to 'album_release_date', and _values_ set to 'Count of candidate'. From here, I filtered the candidate section to display only results for mentions of Donald Trump, to get a pivot table displaying counts of positive, neutral, negative, and total mentions of Trump for each year. 
This data was then used to create the data visualisation shown above.

### Analysis:
The data visualisation shows that the number of times Trump has been mentioned in hiphop lyrics have generally increased, from only 3 total mentions in 1989 and to a peak of 33 mentions in 2013. It also shows that while his general popularity in terms of number of mentions in hip hop song lyrics has increased, sentiments towards him have soured over time. Mentions of Trump from late 80s to the early 2000s were almost exclusively positive or neutral. However, in 2015 there was an explosion in the number of mentions of Trump with negative sentiments, and by 2016 negative mentions of Trump were almost 4 times more common as positive ones. This is no doubt a reflection of changes in how the wider media has portrayed Trump. In the late 80s and early 2000s Trump was mostly seen an image of wealth, with his name popping up on lists like "Ten most admired men and women living of 2011". However since launching his presidential campaign in 2015, he has received more scrutiny for his political views which correlates with the rise in negative sentiments towards him in hip hop. 


## Recurrent Themes in Hip Hop Mentions
This infographic shows the reccurent themes in mentions of all 2016 US Primary Candidates

![Recurrent Themes in Hip Hop Mentions](https://media.journalism.berkeley.edu/upload/2020/08/1597608269940fee7.png)

> This chart was made using Canva. The data was found via a pivot table which  had _columns_ set to 'theme', _rows_ set to 'album_release_date', and _values_ set to 'Count of candidate'. 

## Changes in Sentiments Towards Trump by Theme
> To look closer at how themes in mentions of Trump of have changed, I created another pivot table, this time with _filter_ set to 'candidate' and 'sentiment', _legend_ set to 'theme', _rows_ set to 'album_release_date', and _values_ set to 'Count of candidate'. From here, I filtered 'candidate' to show only Donald Trump, and 'sentiment' to show only positive mentions of Trump.

The result is this chart, which shows positive mentions of Trump by theme:

![Positive Mentions of Trump by Theme](https://media.journalism.berkeley.edu/upload/2020/08/1597609399bf9b6b2.png)

Again, we can see that positive mentions of Trump in hip hop lyrics mostly referred to Trump's money and hotel, which supports my earlier theory that prior to Trump's announcement of his presidential campaign, Trump benefited from an overall positive image thanks to the media's focus on his welath. Post-2015, we can see dramatic drop in references to his wealth and power, and a drop in positive references in general. 



