# Data-Viz-Redesign-Project<br><br>
## Instructions<br>
The objective of this project is to redesign a data visualization (e.g., an infographic, a data visualization in a newspaper, a project report, or a sales report). This will allow you to learn from others, sharpen your critical perspective on data visualizations, reason about design decisions, and attempt to improve data visualizations. <br><br>

## 1. Original Visualization
The original visualizations can be found __[here](https://www.tableau.com/about/blog/2017/4/flex-your-data-skills-makeover-monday-68584)__<br>
<img width="862" alt="screen shot 2017-11-03 at 10 19 24 pm" src="https://user-images.githubusercontent.com/32026039/32402605-265d19a6-c0e5-11e7-8509-d41bb78256db.png"><br>
*Figure.1*<br>
While these two visualization are very clear and easy to understand, I felt that it still required some effort for the viewer to gain full understanding of the data. For example, for the first visualization, it is clear to see the changes in rank of the different skills over the years, but the viewer must move their mouse over to the datapoint in orde to see which exact skill the data is referring to. Also, even though the viewer may view dataset from other countries easible by selecting the country from the drop down menu, it is hard for them to have a comparison of data from each country without having them displayed side by side.
<img width="993" alt="screen shot 2017-11-03 at 10 19 41 pm" src="https://user-images.githubusercontent.com/32026039/32402607-2dd95398-c0e5-11e7-8825-24d5f779c2eb.png"><br>

*Figure.2*<br>
This figure allows the viewer to input key skills they are interested in and displays a chart which illustrates the ranking pattern of the selected skill. This chart blends all of the data together and the only useful information the viewer can get at a glance is ranking change expanding over all three years. Again, the viewer must rely on using the tool tip if they want to see further info, such as the country and specific rank for that year. The graph also blends all data from all countries together; some skills may not appear at all and the median ranking is a half number and this decreases effectiveness of the dataset. Both figures' biggest flaw is that the viewer has the control over how much of the data they want to observe; without moving the cursor, or inputing data fields, they could only view a very limited portion of the data.<br><br>

### Objectives: <br>

>This should not be a visualization to just map current popular job skills, but also potentially make a forecast for the future. For example, how long will cloud-computing be at the top? is it worth it to invest an education based around these skills? Would these skills still be relevant by the time I finish my degree? Should I think about updating my education? These are some type of questions my visualization will attemp to explore.

-Scope:<br>
> Limit to only United States and top 10 skills from year to year.

-Observe trend of the skills
>Skills falling out of favor vs rising popularity of the skills<br>

-Audience: students currently studying the Data related field, and new graduates who are unemployed/actively seeking jobs<br>
> Viz should be forward-looking; make an impact and invoke them to take action

-Action Invoked:<br>
>student/employment seeker will try to take related courses/obtain the skill; or if they already have some knowledge of the skill, they will want to refresh that skill or obtain some related certification.<br><br>

# Version 1<br>
<img width="851" alt="screen shot 2017-11-02 at 10 52 53 pm" src="https://user-images.githubusercontent.com/32026039/32402679-e9306432-c0e6-11e7-9074-d9fa6b6d6b88.png"><br><br>
In Tableau: used dual axis; skill on one side and 'importance' values on another with trend line shown.<br>
For the first iteration, I showed the importance of each skill by taking the inverse number of their original rank; rank 1 skill had the most importance with a value of 10, rank 2 had the value of 9, etc. Skills are sorted by importance, thus the highest ranking skills had the biggest circle and came on top of the list. The trend lines also shows if this skill is either ascending or descending in ranks. This visualization is a improved version over the original Figure 1, since the trend can be observed immediately, and the audience could see the ranked skill names without moving their mouse.<br><br>

However, the visualization is still cluttered; there are too many circles in the frame and the audience might still have difficulty distinguishing one skill from another. There is little difference between consecutive ranks (10 and 9, 7 and 6 etc.) the size of the circles did not make a difference.<br><br>

# Version 1.1<br>
<img width="965" alt="screen shot 2017-11-03 at 4 53 24 pm" src="https://user-images.githubusercontent.com/32026039/32402700-387921aa-c0e7-11e7-93db-11812361249b.png">
<br><br>
This version is a slight improvement over the last iteration; since size of circles were not enough to distinguish small changes in ranking, I decided to use a color scheme to indicate rise/fall of ranking. For skills dropping in importance (ranking) below 6 (thats anything below rank 5), color will change from orange ("hot skill") to blue.

<br>

The problem here is that that if a skill rises a small increment and still falls within the cut-off range (thats above or below 5), color will stay the same. Trend lines in combination of the numbers is still not enough to convey if a skill is rising or falling in ranks. For the next few iterations, I've decided to explor options other than using size of circles and the "importance" value in ranking the skills and go back to using actual ranking values.<br><br>

# Version 1.2<br>

<img width="888" alt="screen shot 2017-11-03 at 6 41 19 pm" src="https://user-images.githubusercontent.com/32026039/32402717-abb6c5dc-c0e7-11e7-88b8-52672cb6808e.png"><br><br>
This version was developed as a intermediate iteration after I've decided to give up the idea of using circle sizes to distinguish ranks; it was also used as part of Lab Assignment 4. What I liked about it was that the skills were labelled and the audience would also get an idea of where the skill is placed in ranking based on position.<br><br>

However, because the mark labelling in Tableau did not allow for rotation, the skill names were placed in very random postions making the visualization look messy and out of order. The colors used as color scheme were also random and not significant.
<br><br>

# Version 2.0<br>
<img width="960" alt="screen shot 2017-11-03 at 4 51 22 pm" src="https://user-images.githubusercontent.com/32026039/32402741-f36abe56-c0e7-11e7-9d0a-66a93d64633f.png"><br><br>
This is the final version of the redesign visualization. I took what I liked most about the original visualizations and added on additional features/info to enhance it. Firstly, the after experienting with different chart styles, I still felt the "bump chart" looked best with this data set; the audience can trace the increase and decrease in ranking or each skill with ease and the spatial lay out of the ranks from top to bottom makes alot of sense as well. I also labeled the different skills unlike the original visualization, and used a set of color schemes which had more significance; red indicates drop in rank, green is increase in rank, and yellow is no change. The exact change in the ranks are also labelled directly on the data points to clarify trend. The change in rank value was calculated manually, as the data set was small; it was result of skill ranking for 2016 minus the skill ranking for 2014. Those skills labelled by gray colors indicates that they dropped out of top 10 rank by 2016. <br><br>

*Future improvements/features:* Reflecting on the final version of the visualization, I feel that perhaps colors chosen were probably not a good idea to convey trend; red and green could also mean the other way around, as they do in stocks (green is decrease, red is increase). The numbers could also be misleading; without reading the caption, the audience might not understand that it is signifying overall change in ranking. I could perhaps use symbols to indicate trend; red downward arrows for overall decrease in ranking and green arrows for increas in ranking. The exact value could also be labelled beneath the symbol to give a solid indication of the trend (positive/negative). Symbols in combination with the color might clarify ambiguity associated with different interpretations of the colors, symbols etc.

Since I set the audience limited to students in the United States with the intent of staying in the states to work after graduation, I did not use any of the data from other countries. It would be interesting to view the ranking trends for other countries as well, and gather insights on career possiblities overseas. But personally, I feel like this dataset is best utilized for data in the United States,because Linkedin started up in the Bay-Area and it is a well-known networking tool in the country. To make the dataset more accurate, one can take into account the percentage of the population that actually uses Linkedin. It might also be worthwhile to wait for Linkedin to release a larger list for 2016 (current only has top 10 skills) to be able to do a deeper analysis/long term projection of which skills might be persistently ranked for the future and which might eventually drop out of top 25 entirely.If a visualization is impactful, it will invoke the audience to take action and start acquring some of the skills;this itself will be a time-consuming process and they would not want to finish a degree and realize some skills they have learned have dropped out of favor. Another flaw to the dataset that might mislead the audience is that although some skills such as object-oriented programming languages are not on top of the list, it is still a crucial pre-requisite to other skills. <br><br>

The answers to the questions I have came up with in the objectives at the beginning of the project remain partially unexplored; we need alot more data to be able to accurately visualize a trend with a futuristic outlook. However, what is sure is that information/data related skills are still very relevant and rising in ranks; when skills do fall in ranking, they will not fall too far down for them to be irrelevant(slow descent). Also, almost all top 10 skills are software-related. Thus, if a student is in/around the parameter of the software field, they can be sure that they are on track in pursuing a successful career.<br><br>

*Video: __[Youtube Link](https://www.youtube.com/embed/DoNOnv6_1fE)__<br>
*cover image credit: https://goo.gl/images/pYKcSE <br><br><br>

### Sources:
1. Top Skills on Linkedin: __[Makeover Monday Blog Post](https://www.tableau.com/about/blog/2017/4/flex-your-data-skills-makeover-monday-68584)__<br>
2. Top Skills on Linkedin Data Set: __[Download Link](https://onedrive.live.com/view.aspx?resid=43EBDBC5D5265516!11505&ithint=file%2cxlsx&app=Excel&authkey=!AMgM7CPfLy7rocE)__<br>
3. #MakeoverMonday, Linkedin Top Skills Tweets page: __[Link](https://twitter.com/i/moments/857430926015451138?lang=en)__<br>
4. A updated version of the ranking can be viewed here (an older dataset was used for this project): __[Link](https://learning.linkedin.com/week-of-learning/top-skills)__<br>


