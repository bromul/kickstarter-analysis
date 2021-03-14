# Kickstarting with Excel

## Overview of Project
This project analyzed Kickstarter data to provide insight into crowdfunding and producing plays.

### Purpose
Our friend Louise created a play and wanted to know the best conditions and ways for her to successfully fund it. By analyzing Kickstarter data on projects' goals, pledges, and launch dates, we have produced this report outlining criteria she can use to increase her chances of successfully funding her play.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To determine the rates of outcomes based on the date theater projects were funded, we created a pivot table that stratified 'successful', 'failed', and 'canceled' projects by month. 
Through this, we found that theater projects were most successfully funded during the months of May and June, with 111 and 100 projects funded respectively. The amount of successfully funded theater projects tapers off throughout the rest of year when in December the number of projects that met their funding goals and failed their funding goals are about equal. ![Theater Outcomes by Launch Date](https://github.com/bromul/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
In Louise's case, it would be better to launch her theater project within the months of May or June - and to heavily avoid launching during the winter months. 

### Analysis of Outcomes Based on Goals
By binning theater project goal amounts in ~$5,000 increments, we were able to calculate the precentages of projects that were 'successful', 'failed', or 'canceled' by the initial goal. 
From this, we found that a theater project's set goal seemingly plays a large role in the whether or not it is successfully funded. As the stated goal increases, the chances of successfully funding the project decreases. The only exception to this trend appears to be projects in the range of $40,000 to $49,999, which has a success rate of 62.5%. ![Outcomes Based on Goals](https://github.com/bromul/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
However, without having dug deeper into the data and into these projects in particular, I believe it seems likely that this is due the lack of many projects within this range (small n) as well as the possibility that these theater projects were created by established artists or were 'staff picks', and should not be taken as indicative of the whole. 

### Challenges and Difficulties Encountered
During this analysis, I ran into some issues creating the pivot table. Specifically, ensuring that the data was stratified by months. I was able to solve this issue by remembering the ways that Excel can separate time-dependent data within years, quarters, months, etc. 

Additionally, while calculating the percentages, it didn't immediately occur to me that I could - and should - lock specific cells when copying my equations over. Once this was remedied, however, with a '$', creating the table became immensely easier.

## Results

### Conclusions from Analysis
From this analysis, there are a few conclusions we can draw regarding a theater project's outcome based on its initial launch date and its goal amount.

For the launch date, we can conclude that the best months to launch a theater project on Kickstarter are May and June, as these two months showed the highest rate of success. Conversely, a theater project should not be launched during the winter months - and especially not Decemmber. Curiously, the number of failed and canceled theater projects remained fairly steady throughout the year, so the variation between months with greater and lesser success cannot only be explained by an increase or decrease in the amount of projects posted at any given time.

For the goals, we can conclude that the rate of theater projects being successfully funded is inversely correlated with the project's stated goal, that is, its success decreases as the goal increases. As stated earlier, the only exception to this trend appears to be projects within the $40,000 to $44,999 range, but there's no evidence as of now that that range should be treated as a break from the trend. Additionally, we can conclude that, while remaining fairly steady between goals of $0 to $34,999, theater projects are canceled more often at goals at or above $35,000. This suggests that projects with larger goals have a harder time being met.

### Limitations of Dataset
There are, however, some limitations to the dataset itself. At around 4000 listed projects, it may be too small of a sample to properly draw conclusions from. This limitation is further compounded by the fact that the dataset does not only concern projects of interest, i.e., theater projects, which further reduces the gross number of projects worked with. While this may not break our analyses of theater project outcomes - since theater may make up a small portion of Kickstarter projects to begin with - it is an issue we should be aware of when using this analysis. 

Furthermore, although this dataset contains the amount pledged to a project and the number of backers, we cannot see individual donations to each project. This would allow us to determine if irregularities we found, e.g., projects with goals between $40,000 and $44,999 having higher rates of success, were due to large, single contributions rather than true 'crowdfunding'. 

### Future Analysis
While we were unable to do further analysis of the data at this time, there are other potential relationships we could look at to deepen our analysis. The creation of tables that showed a theater project's success rate and/or amount pledged by whether or not the project was a 'staff pick' or 'spotlighted' might elucidate our analysis to the processes in which certain projects were funded, e.g., are successfully funded projects with high goals more likely to have been a staff pick or 'in the spotlight'?

We could also create tables or visualizations of backer count versus rates of success. This would give us more information on whether the success of a theater project tends to rely on many people backing it or just a few 'devoted fans'. 

Alternatively, we could perform a similar analysis to what we did for theater projects, but with other categories and subcategories. Creating these tables and graphs could give us broader insight into how Kickstarter projects function in general. 


