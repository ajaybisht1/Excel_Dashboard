<img width="782" alt="image" src="https://github.com/ajaybisht1/Excel_Dashboard/assets/146637154/eab475f1-4e57-42f8-8fe1-c750cf78e20a"># Work Status Dashboard
<br>

### What is work status dashboard?
- This is an automated dashboard which was created by me to keep track of daily work status within my team

### What purpose does it server?
- This is a combined dashboard which replaced multiple individual dashboards that were being shared on daily basis within the team
- All the activities listed in multiple sheets within this dashboard are discussed in daily team call and this dashboard displays both work completed and work pending status.

### What were the visible benefits of making this dashboard?
- This was found useful by seniors and pushed for implementation in many teams in my organisation which saved approx 20hours of manual work each week 

### What I learned while making this dashboard?
- I learned how excel workbook can be linked to **micorsoft access database** to retrieve the data just by refreshing the worksheet.
- I learned the implementation of **macro** in real time case scenario
- I learned the use of **conditional formulas** and how they can be used in real time to manipulate data
- I learned to **protect excel sheets** and workbook structure so that file can be protected against any unwanted changes being made
- I learned the use of charts to **visualise the data**

<br>
<br>
<br>

## Working of Dashboard

<br>

Dashboard has 7 worksheets
#### Worksheet 1 (How to use) - This worksheet just explains how this dashboard needs to be prepared for daily use
#### Worksheet 2 (Pending Activity 1)

   <img width="652" alt="image" src="https://github.com/ajaybisht1/Excel_Dashboard/assets/146637154/6d790239-139c-4ec5-822d-78f55b9b995a">

- When we create this worksheet it starts to display pendency of work in activity 1 for each analyst
- We have used Macro to create two buttons "Clear" & "Refresh" that help in clearing old data and refreshing pivot with new data once loaded
- In column N we have used Vlookup to fetch name of analyst who is responsible for completing that activity.

#### Worksheet 3 (Pending Activity 2)

<img width="523" alt="image" src="https://github.com/ajaybisht1/Excel_Dashboard/assets/146637154/fb36d929-b588-40b6-9d87-ea7b548f7405">

- This worksheet shows pendency of work in activity 2
- In above image there are 23 pending activities but we do not know which analyst needs to do that. To know that you have to enter store number in cell "J5". As soon as you do that cell "J6" will return the name of analyst who is responsible for working on that store. This feature was very useful during daily meetings when team leads quickly wanted to know which analyst is leaving work pending

 #### Worksheet 4 (Database_query_name)

 <img width="823" alt="image" src="https://github.com/ajaybisht1/Excel_Dashboard/assets/146637154/209c8026-e4bf-4636-9c63-972e0a5fa77d">

- This worksheet is linked to access database and works as a source for upcoming worksheets. On just a single refresh it gets updated to the current
- Column A to G are retrieving from database and column H to N are manually added which have formulas such as Vlookup, IF error, Today these columns are useful to created next few worksheets.

#### Worksheet 5 (Pending Activity 3 Ageing)

<img width="782" alt="image" src="https://github.com/ajaybisht1/Excel_Dashboard/assets/146637154/12a8a861-88cb-4fb7-8e17-e69fa334b6d7">

- This worksheet has count of pending work in activity 3 with the ageing and analyst allocation.
- This is really helpful for quickly glancing over the pendency status
- The data source for this worksheet is coming from Worksheet 4 (Database_query_name) which is a replica of data base so we can say this pendency is coming directly from database.

#### Worksheet 6 (Pending Activity 3 Ageing)
