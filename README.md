# Animal-Shelter-Analysis
Animal Shelter Operations Analytics 
In this Project, Animal Shelter Intakes and Outcomes dataset from the City of Long Beach Animal Care Services.

I leveraged my DAX skills to create measures and generate insightful visualizations. To finish off, I brought it all together in a sophisticated business dashboard to communicate insights to the Stakeholder.

**Project Steps**
1. Know the Objective
2. Understand the dataset
3. Data Cleaning
4. Data Modeling
5. Exploratory Data Analysis
6. Report Design

Lets dive in!

**Step 1: Know the Objective**

*Business Objective*:
The objective is to create a Power BI report that uncovers operational trends, improves understanding of live-release performance, and supports data-driven decisions related to shelter capacity, resource planning, and animal welfare outcomes..

**Step 2: Understand the dataset**

The Dataset is Animal Shelter Intakes and Outcomes from the City of Long Beach Animal Care Services. The dataset includes detailed information about each animal entering or leaving the shelter, such as species, intake type, condition, outcome type, and length of stay.
The dataset has just 1 Table named Animal Shelter Operation.
After carefully going through the data, i loaded the data into the PowerBi desktop app for data cleaning.

**Step 3: Data Cleaning**

Data Cleaning is one of the most important process in data analysis. if you do not clean your data properly, your analysis wont be accurate and it will affect the insight you will generate.
i went through the ETL process which is, i extracted my data first then transform it before loading the data. The transformation of the data which also means cleaning of the data was done using power query.
The data is not that messy so i checked for the duplicate value, missing value and the data types of the column name to see if it really correspond with the column name.

**Step 4: Data Modelling**

Since the Dataset has only 1 Table, i just connected the Table Animal shelter Operation to the Calendar Table i created with DAX, The Dataset was joined with the Calendar Table via the Intake date and outcome date.
below is the data model of this project
![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Data%20Model.PNG)

**Step 5: Exploratory Data Analysis**

After doing the data modeling, then i created some measures using DAX formular to answer some of the question asked.

1. 	How intake and outcome patterns evolve over time?
   To answer this question, i created a line chart to visualize the month against the Intakes and Outcomes Trend. By this, you can toggle among the month to see how intake and outcome changes on monthly basis.

   ![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Intake%20and%20Outcome%20trends.PNG)

2.  Which animals face longer shelter stays or higher risk of non-live outcomes?
   To answer this question, i created a clustered column chart to visualize Animal type against Average length of stay. Rabbit is the animal with the highest length of stay followed by Guinea Pig, Cat e.t.c
   ![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Animal%20LOS.PNG)

3. Which types of pets are adopted most often?
   To answer this question, i created a Stacked Column chart to visualize Animal Type against Adoption Count. i created a DAX measure for adoption count, which i potted against Animal type. Cat is the most           adopted pet followed by dog.

   ![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Adoption%20pet.PNG)

4. Which species, age groups, or breed types have higher or lower live-outcome rates??
   To answer this question, i created a Clustered Column chart to visualize Animal Type against Live Outcome Rate. mind you, i already use DAX formula to calculate live outcome rate. Amphibian is the animal with    the high live outcome rate followed by Livestock the  Guinea pig e.t.c.
 
   ![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Animal%20with%20high%20LOR.PNG)

5. Which intake sources contribute the largest volumes, and what does this imply for community outreach or prevention programs?
   To answer this question, i created a Clustered Column chart to visualize Intake Type against Total Intake. Animal that strayed into the Animal shelter has the highest number followed by animal from wildlife      e.t.c.
 
   ![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/intake%20source%20with%20highest%20volume.PNG)

6. Are there animals that return to the shelter more than once?
   To answer this question, i created a Clustered Column chart to visualize Animal Type against Repeat Animals. i created a DAX formula to calculate Repeat Animals. Dog is the most animal that return to the         shelter more than once followed by Cat and Rabbit e.t.c

   ![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Repeat%20Animals.PNG)

All the question was answered and visualized with the necessary charts.

**Step 6: Report Design**

I created some KPI's which are Card visuals, the following KPI's are created: Total Intakes, Total Outcomes, Live Release Rate %, Death Rate, Average Length of Stay, Animals in Shelter, Adoption Rate, Euthanasia Rate, Repeat Animal Rate, Transfer Rate, Return to Owner Rate. 
A line charts of Intake and Outcome Trend was created, a donut chart of Total Intakes by sex was created, a stacked column chart of total intake by Age category was created.

Conclusively, I put all the visuals of the question asked into a report template. The Report has 2 Pages, i created a “Overview” page which is the Home Page and provided users with quick access to navigate between pages in the report while the other page is Adoption Analysis Page.

Below are the images of the 2 Page Reports.
![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Overview.PNG)
![](https://github.com/phuad23/Animal-Shelter-Analysis/blob/main/Adoption.PNG)


Click [Here](https://app.powerbi.com/links/kkPO4N8oaU?ctid=d5bc17d2-4910-4403-86b9-672f3274f2f9&pbi_source=linkShare) to interact with the dashboard. 
