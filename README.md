# Kickstarting with Excel

## **Overview of Project**

Louise is a playwright who wants to launch a play with funding provided through a kickstarter. We are going to do everything we can with the information available to improve her odds for success.

### **Purpose**

The purpose of the project is to help Louise understand historical trends in kickstarters, for plays in particular, to increase the chances of success of her own kickstarter.

## **Analysis and Challenges**

We sought to isolate the most relevant information available to find a successful strategy for Louise's kickstarter. After exploring the data and analyzing it from a few different angles, the there were a couple of factors that impacted the odds of a successful kickstarter that stood out. Those were the size of the goal, and the launch date.

We performed our analysis by focusing on the Theater kickstarters, particularly for the 'Play' subcategory. This required parsing the 'Category and Subcategory' fields into two new fields named 'Parent Category' and 'Subcategory' so that we could explore theater plays in isolation from the other theater kickstarters, since it is most relevant to Louise's needs.

From here, we pursued two different analyses: outcomes for theater kickstarters based on their start dates and outcomes of kickstarters for plays based on their funding goals.

The most challenging part of this data set was converting the date values from their Unix Time Stamp format into a commonly used date format. The Unix Time Stamp format is not very legible and the formula for its conversion is not simple:

Unix Time Stamp format:

![alt text](https://user-images.githubusercontent.com/75325334/102724339-dd6bcd00-42dc-11eb-9688-35ddd52c26ea.PNG)

Conversion Formula:

![alt text](https://user-images.githubusercontent.com/75325334/102724340-df359080-42dc-11eb-9150-88cfaefe4a27.PNG)

### **Analysis of Outcomes Based on Launch Date**

We analysed outcomes based on launch date by pivoting the data into a table that looked at successful, failed, and cancelled kickstarters grouped
into months irrespective of the year they were launched in. This gave us insight into the best and worst months of the year to begin a Kickstarter
campaign. We displayed this information in a line graph for effective visualization.

### **Analysis of Outcomes Based on Goals**

We analysed outcomes based on goals by grouping all of the fundraising goal amounts together on an incremental scale. On this scale, we are
able to see the number of successful, failed, and cancelled kickstarters and analyze the outcomes based on the the amount of the goal. 

### **Challenges and Difficulties Encountered**

The most challenging aspect of this analysis was the formula required in the 'Outcomes Based on Goals' tab to isolate Plays within a given Goal range
by outcome. This statement must simultaneously meet 3 conditions in each instance which was, at first, a bit of a challenge to wrap my head around.

Screenshot of an example of the formula and the entire table:

![alt text](https://user-images.githubusercontent.com/75325334/102724335-da70dc80-42dc-11eb-8372-025d8a2a53fc.PNG)

## **Results**

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The analysis of outcomes based on launch date shows us that the May, June, and July are the most successful months to begin a Kickstarter historically. The month of May in particular stands out as the best historical month to begin a Theater kickstarter. May had the highest proportion of successful kickstarters, as well as the highest number of successful kickstarters. 

We can also conlcude that kickstarters beginning in September through March have the highest likelyhood to fail.

- What can you conclude about the Outcomes based on Goals?

The analysis of outcomes based on goals shows us, in the simplest terms, that the lower the goal the more likely the kickstarter is to be successful.
Although the proportion of successful kickstarters is notably high in the $35,000-$49,999 range I would not place too much importance on that due to the 
extremely small sample size.

- What are some limitations of this dataset?

One limitation of the dataset is that it does not list every single donation and the relationship between the kickstarter hopeful and the donator.
Understanding instances where relationships to certain donors has given kickstarters a comparative advantage would help us understand Louise's relative chances for success better, because we could look at single instances of very high donations from special parties that we know Louise would not receive. This would also allow us to see exactly how the donations were distributed along a timeline.

- What are some other possible tables and/or graphs that we could create?

We could go further into our analysis by looking at the impact that kickstarter campaign duration has on outcomes, and plot those campaigns on a timeline in order to see if it is not only the month that the campaign begins in that impacts chances of success, but also the months during which the campaign is ongoing and the ideal duration of a kickstarter campaign.
