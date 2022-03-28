# kickstarter_analysis
## Overview of Project
We are organizing, sorting, and analyzing relevant crowdfunding campaign data for several types of entertainment categories to determine if there are specific elements that contribute to successful campaigns. 
### Purpose
The purpose of this analysis is to identify the characteristics of successful campaigns for projects within the theater category and specifically, plays. We are using these insights to help our client plan her own goals and parameters for her crowdfunding campaign for her upcoming play to give her the best chance of succeeding. 

## Analysis and Challenges
The client provided us with a large data set that detailed information on previous crowdfunding campaigns. In the first phase of the analysis we had to decide which pieces of this data set were the most relevant to our clients project. Because the client is working on a play, we wanted to isolate the pieces of the data set that fell within entertainment productions and more specifically the theater/play category. This was an important distinction to make as some of the other categories such as film & video/television had much higher budgets and different elements unrelated to the theater industry that would sku our data.

Each category and subcategory have unique variables to consider for when setting a budget. After filtering and sorting the "Kickstarter" sheet to show the theater data we wanted to focus on, we noted the crowdfunding campaign categories and subcategories were lumped into the same data cell. Because the theater category has several different subcategories, it was important to split the category/subcategory information into two new columnn so we would be able to isolate the plays and factors impacting the projects that most closely related to our clients's upcoming play production. 

### Analysis of Outcomes Based on Launch Date
The first piece of information we examined after isolating projects within the theater category is the success of campaigns based on their launch dates. The launch date information from the original dataset were in unicode. In order to make this information readable we had to convert them into standard mm/dd/year formatting in a new column. This made it easier for us to group the dates by month or year accordingly.

We wanted to dig a little deeper and see if the timing of launching the campaigns had any effect on whether or not they had a successful outcome. We exported the filtered theater data into a pivot chart and created a line graph depicting the number of theater campaigns that were successful, failed, for each month of the year. 

/assets/Resources/Theater_Outcomes_vs_Launch.png

The chart referenced above showed that crowdfunding campaigns launched in April for the theater category had the highest number of successful campaigns. The number of succesfuk outcome for theater campaigns launched after April steadily decline into September before we see a slight increase before it continues to decline. The number of failed outcomes for the Theater campaigns appears to be relatively similar throughout the year. The number of failed theater crowdfunding campains appears to peak in October. 

Based on these findings we would recommend our client launch her crowdfunding campaign in April, as that seems to have the highest concentration of successful campaigns for the theater category. 


### Analysis of Outcomes Based on Goals
The biggest factor we wanted to examine in this data set is how the goals set at the beginning of crowdfunding campaign impact the success of the production since our client will be using our analysis to determine how to set a goal that is attainable and will set the production up for success. For this portion of the analysis we isolated the subcategory plays specifically to get the most accurate picture for our client. 

We created a new sheet called "Outcomes Based on Goals" and broke down the goals for play campaigns into 8 ranges (see below) and calculated the percentage of successes for campaigns in each goal range. Our client wants to ser her campaign goal to $10,000 we paid special attention to the percentages of successful outcomes compared to failed outcomes within that range 10,000 to 14,999). 

Overall, it appeared that productions with smaller goals had the highest overall success rate. Play productions with goals of $10,000 and below make up the bulk of the data, with very few plays with higher budgets. Our clients goal relative to most other play productions is on the higher side. For the $10,000-14,999 goal category, 54% are successful and 46% fail. It would be in her best interest to keep her goal as low as she can without compromising the quality of her production. 

/assets/Resources/Outcomes_vs_Goals.png

### Challenges and Difficulties Encountered
There were some challenges with converting the original dataset into usable information for our purposes. For example, in order to isolate the data we wanted we had to create new columns for the categories and subcategories. Lumping information togther makes it harder to sort and filter the data by the information that was relevant to our client. The unicode formattiing was also a challenge because the date information was an ambiguous number until we were able to convert it into a readable format. 

## Results
After examining the impact of launch date and goals on theater campaigns success, we can identify a couple of meaningful factors that may contribute to the success of campaigns similar to our client's upcoming production. 
- What are two conclusions you can draw about the Outcomes based on Launch Date?
After examining the impact of launch date on theater campaigns success, we can identify a couple of meaningful trends. It appears April is has the highest concentration of successful theater campaigns relative to the months throughout the rest of the year and may be the best time to start a campaign. The highest concentration of failed campaigns are launched in October, but remain relatively steady throughout the rest of the year. 

- What can you conclude about the Outcomes based on Goals?
It appears there is a higher concentration of plays with crowdfunding goals under $15,000. The play campaigns with the highest percentage of successful outcomes have goals below $5,000. From there as the goal increases, the percentage of successful campaigns declines. 

- What are some limitations of this dataset?
I would say one of the biggest limitations of this data set is it focuses mostly on quanititative information. Other factors, such as the quality of the production and interest each campaign is able to generate also would have a large impact on the success of reaching a goal. If the production is unable to gather enough public interest, that would negatively impact it's ability to reach it's campaign goals. 
- What are some other possible tables and/or graphs that we could create?
I think it would also be helpful to create a table and graph that depicts the amount of time the successful and failed campaigns had between it's launch date and deadline to reach their goal. This would give us some insight into how much time it takes to run a successful campaign and give us another suggestion to help our client plan for success. 
