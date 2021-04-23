# An Analysis of Kickstarter Campaigns
Performing an analysis on kickstarter data to uncover trends
Data were pulled from Kickstater to introduce students to using Excel, basic Excel functions, and basic stastical analyses. 
Specific data pertaining to Louise's desire to start a kickstarter for a musical in Great Britain. Pivot tables and box plots were used to aid in the analysis. 
Louise has a target of aproximately $4,000 to fund the musical, and analysis of successful to failed musicals suggest that the funding goal is a reasonable target. The box plot showed that the mean musical goal was approximately $4,000 and was within the IQR. The box plot is presented below:
![Box_Plot_Musicals_GB](https://user-images.githubusercontent.com/82423123/115622326-4ed48000-a2bd-11eb-9b4f-2434fd232067.png)


**Analysis of Kickstarter Data**

1) This Kickstarter data was analyzed to determine if Louise's goal of raising $5,000 was a realistic goal for her play. To come to a conclusion, relationships between the goal amount, success of the Kickstarter, location, and launch dates were analyzed. 

2) Initially, not all of the data were in usable formats; explanations of data cleaning are included below. 

-The launch and deadline dates were in unicode format and thus not intuitively readable, to convert , the following Excel formula was used: `=(((K96/60)/60)/24)+DATE(1970,1,1)`, where "K96" is the cell containing the date to be converted. 

-Additional challenges involved the use of pivot tables to quickly perform summary statistics; the challenge arose from an unfamiliarity with pivot tables and was overcome by trial and error and supplementary learning. 

Analysis was performed using the aforementioned pivot tables to quickly and intuitively analyze the relationship between the outcomes of theater Kickstarters and their launch date. Images of the pivot table results and resuming graph and presented below. 

![Theater_Outcomes_Launch_Date_Table](https://user-images.githubusercontent.com/82423123/115929454-7a867000-a44d-11eb-84f5-74673312979c.png)

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/82423123/115929506-8bcf7c80-a44d-11eb-8097-871f636425f6.png)

Lastly, analysis was performed on the relationship of the outcomes of theater Kickstarters and the target monetary goal. Date were filtered for "plays", then using the '=countifs' formula in Excel, the number of successful, failed, and canceled theater Kickstarter campaigns were calculated, then percentages of that extracted data were calculated for ease of viewing the data. The resulting graph is presented below. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/82423123/115929527-95f17b00-a44d-11eb-9386-b5b704919895.png)

3a) Analysis of Theater Outcomes by Launch Date

Analysis of theater outcomes by launch date demonstrated a clear spike in the number of successful campaigns started in May, with a consistent linear drop-off over the summer, followed by another drop-off from October to December; these results are presented above in Section 2. As the graph analyzes by month and adds all data from each year together, further analysis was performed to determine if there was the same relationship through time. The resulting graph is presented below.

![Theater_Outcomes_vs_Launch_Through_Time](https://user-images.githubusercontent.com/82423123/115929552-9ee24c80-a44d-11eb-8c27-76d8c0e2cb78.png)

As seen on the above graph, the same spikes of successful campaigns seems to occur in May, the drop-offs following the May spikes do not seem to be as consistent through time; however, winter seems to have a consistently lower number of successful campaigns. There is apparently is cyclical relationship with more successful campaigns in the early summer and the lowest number of successful campaigns in the winter. 

Additionally, there seems to be no failed campaigns from 2010-2013; however, this is dubious and is possibly a result of inadequate data or that failed campaigns were not recorded during those years. As such, it might be prudent to exclude date prior to 2014 for making decisions. 

After analysis of successful campaigns through time, the trends of successful vs. failed campaigns seemed to follow each other closely, and further analysis was performed to analyze this relationship. The resulting graph is presented below. 

![Relative_Percentages](https://user-images.githubusercontent.com/82423123/115929584-aace0e80-a44d-11eb-90a5-d59d608da3ce.png)

Note that dates before 2014 are excluded as there are no records of failed outcomes. This graph demonstrates that the increase of successful outcomes could just be due to the increase in total number of campaigns initiated; for example, while July 2014 had the highest number of successful campaigns in 2014 it also had a relatively large decrease on the percentage of successful campaigns, approximately a 15% drop from June 2014 (~70% to ~65%). While the cyclical nature isn't as apparent as in the previous graphs, there still does seem to be a higher success rate around May. 

3b) Analysis of Outcomes Based on Goals for Plays

The outcomes based on goals chart is presented again below. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/82423123/115929611-b588a380-a44d-11eb-99cf-918bdbaab7b4.png)

Initially, is appears that there is a good relationship between the goal and chance of success, with the higher the goal, the lower the chance of success up to the $25,000 to $30,000 range. There does not appear to be a clear relationship after that range. To further analyze possible relationships, a second chart was made plotting the total number of projects on the same chart; it is presented below. 

![Outcomes_Goals_Total_Projects](https://user-images.githubusercontent.com/82423123/115929631-bd484800-a44d-11eb-9a0d-268fe17468f0.png)

As clearly demonstrated, the number of projects in each category drops off substantially; with fewer data points, the data is more prone to large fluctuations and is less reliable. It is recommended that conclusions only be drawn on project categories with sufficient data. 

However, Louise's play is in the $5,000 to $9,999 category which has sufficient data; as such, it appears that, all other factors equal, she has approximately a 55% chance of her play being funded. 

3c) Limitations of the Dataset

One limitations previously described is the lack of the number of failed campaigns prior to 2014; while it is possible that all Kickstarter campaigns for plays launched in from 2009 to 2014 were successful, it seems doubtful	and calls into question the quality of older data. 

Another limitation is the exposure of the Kickstarter; are Kickstarts with more exposure more likely to succeed? Or who backs each Kickstarter (e.g., a theater company vs. single person). 

There are additional factors that could affect the success of the Kickstarter campaign that are not included in this dataset. 

3d) Additional Graphs to Include

Additional graphs were included in the analyses provided in sections 3a and 3b. However, additional graphs displaying the relationship of the success of the campaign vs. buzz-words in the blurbs or play name, the success vs. number of views on the webpage/amount of money spent promoting the campaign. 
