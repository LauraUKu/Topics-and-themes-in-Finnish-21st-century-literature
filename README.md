THE MOST COMMON TOPICS AND THEMES IN FINNISH LITERATURE PUBLISHED IN THE 21ST CENTURY
(FROM KIRJASAMPO.COM)

This project is an analysis on the most common topics and themes appearing in the metadata of Finnish (language) literary fiction published in the 21st century so far. It is done by analysing the most common index terms associated to the literature. The goal was to find the overall most popular topics/themes for the last two decades, but also to compare possible differences between originally Finnish works and translations, as well as to see if there is some significant variation during the years. The data is collected from Kirjasampo.com, the largest Finnish literature webservice that is based on Finnish library collections of fiction and their linked data. 


DATA, METHODS AND PROCESSING

For the analysis, I used two separate data packages that were cut from a larger Kirjasampo.com -data set. The first one consisted of all books published 2000-2019 with the metadata of title, year of publishing, publisher, author, original language, form/genre and an ID-link. The second one held all the index terms associated with these books, together with the respective ID-links. The original books-file covered 34 896 books (20 158 orig. Finnish & 14 738 translations to Finnish), while the index term-file provided a mix of 372 408 terms (with 8834 individual terms).

Using OpenRefine, I transferred the “year” and “original language” information from the books-file to the index term-file by using the cross() command in the shared ID-link column. Next, the combined project file and its data had to be pre-processed by cleaning out all the literature forms and genres that were of no interest regarding the analysis of topics and themes. The excluded index-words consisting of terms like “romaani” (novel), “runot” (poems), “essee” (essay) etc., that would only distort the results of the analysis. I also changed the ä and ö letters back to normal, removed the ID-links, and fixed a random typo from year “208” to “2008”. After pre-processing, the data was down to 256 418 terms (with 8393 individual ones). In addition, I made too extra files containing only the originally Finnish books and only the translated books, to help the comparison. 

The analysis itself was done by a combination of both OpenRefine’s faceting-feature and the visualization tool Palladio. In palladio I organized the index-words by frequency, thus finding the most common ones. I was also able to compare the frequencies between the translated and originally Finnish books. I copied the top 70 index word comparisons on an excel file for a clearer overview.  In OpenRefine it was easier to examine the differences between separate years by creating yearly facets, because it didn’t freeze with the large datasets, as palladio occasionally did. OpenRefine also provides the possibility to search for groups of words (for example all index terms that include the word love in any part of the phrase or word).


RESULTS

The top 10 most popular topics/themes for the whole period of 2000-2019 were the following: 

	   FINNISH	                TRANSLATIONS TO FINNISH	          ALL
1.	huumori 1941 / 3289	      kaupungit 1367 / 2847	           huumori 3289
2.	kaupungit 1371 / 2847	    murha 1221 / 1976	               kaupungit 2847
3.	naiset 1079 / 2062	      tytöt 1208 / 2057	               ystävyys 2228
4.	ystävyys 1044 / 2228	    ystävyys 1127 / 2228	           naiset 2062
5.	ihmissuhteet 1015 / 1675  huumori 1093 / 3289	             tytöt 2057
6.	seikkailu 951 / 1881	    eläimet 1046 / 1849	             murha 1976
7.	arkielämä 929 / 1267	    naiset 954 / 2062	               seikkailu 1881
8.	tytöt 836 / 2057	        salaisuudet 880 / 1569	         eläimet 1849
9.	maaseutu 749 / 1104	      seikkailu 793 / 1881	           ihmissuhteet 1675
10.	murha 741 / 1976	        rakkaus 641 / 1282	             salaisuudet 1569

Humour, cities and friendship are dominating the top three. They are topics/themes that are adaptable to a variety of different forms and genres of literature, and speak to readers beyond age and gender, which makes the result very logical. Some of the most popular literary genres are also quite easy to figure from the top 10. There is adventure, murders, love and relationships, some common topics for traditional novels, thrillers and detective stories.

There are not major differences between translations and original Finnish literature. However, something that stands out is the topic of the countryside. In the Finnish literature data, it is placed 9th, while the translated side holds it on spot 41. The Finnish topics also emphasize settings like everyday life, nature and villages, which is understandable, because that is something that would most likely be more relatable when written from a Finnish perspective.

The most interesting observation in the whole project was the clear difference between men and women. The topics of girls and women compared to boys and men, showed a huge gap between the two genders. The females constituted a total of 4119 index words, while the males were left with 2281. Boys and men were ranked 12th and 25th compared to the female counterparts’ 4th and 5th. There seems to be a lot more literature aimed to or written about women/girls. This correlates interestingly to the political debate and concern that boys/men in Finland do not read anymore.

The most frequent topics and themes did not vary significantly when compared between separate years. The data itself had some interesting features though. The amount of index terms increases slowly but steadily by time, but there is a clear jump in the year of 2012, when the total amount of topics and themes temporarily almost triples compared to 2011 or 2013. The same happens at 2016-2017. However, this does not apply to the number of books published, for that number smoothly increases from around 1200 to around 2000 books per year, with no apparent anomalies. This temporary jumps in the amount of index terms per book need to be considered before making any greater conclusions on yearly variation.

I did also some targeted searches in OpenRefine for a couple of hot topics of the last few years’ public discourse in Finland, to see if there were some interesting correlation. The search word “pakolais” (refugee) resulted in a correlation to the 2015 refugee crisis. The number of refugee-related topics were under 10 counts on other years, but from 2015-2018 it peaked at 19-45 counts of topics per year. For comparison, topics that contained “maahanmuut” (immigration) grew a bit more moderately and steadily throughout the decades. Another interesting example is “sosiaalinen media” (social media), which appears for the first time in 2010. The variety topics and themes seem to generally become more global along the way. Interestingly, “kansainväli” (international) peaks every three years starting from 2001, until the number settles to a steady growth after 2012. It might be affected by the EU-politics as well as the national elections.


CRITICAL ANALYSIS

Some of the index words did not have information about the original language or the year of publishing, which excluded about 10 700 objects from the language and the year comparison. It is also necessary to point out that some of the topics and themes in the datasets were distributed to different index terms even though they could be grouped as one (ex. “ystävät”/”ystävyys”, “perhe-elämä”/”perheet”/”äidit”/”isät”/”sisarukset” etc.). This most likely has caused some bias in the results. For the future, it would be interesting to further categorize coherent groups of themes. 

What comes to the research question of the most common topics/themes in Finnish literature, this type of data with index words is always somewhat biased. Different books have different amounts of metadata, the terms are subjectively chosen by someone, and something is often left out. With a dataset as large as this, also the cleaning process is more difficult, which means that the data might still have some index terms that should not be categorized as topics or themes. 
