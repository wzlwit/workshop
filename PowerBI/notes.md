# notes:

possible to add tile of 'web content'. ie, there are some video online,  this video can be added as a tile to dashboad

In order to confirm region is populated for every author, you need to use the column profile tool to understand the distribution for the region column. Additionally, the default Power Query profile is only done on the first 1,000 rows. You need to enable column profiling based on the entire dataset to see all 2,500 authors.

*Deployment pipelines* allow you to manage the lifecycle of your organizations content

Writing a SQL statement to filter the rows prior to loading is the only option that will minimize data load time.

You need to create a visual that compares revenue and cost over time. What type of visual should you use?
- Line charts are used to visualize change over time

The web content tile allows you to add and customize any HTML content, like websites. Web content tiles preserve the functionality of the page so you can access other videos on the site. The video tile only allows you to post a single video

Using parameters allows you to easily switch between different tables and schemas in a data source or database

Contributors can update reports in a workspace and update an app. However, they cannot add other users to a workspace

Members can assign member roles and below

Azure Blob storage queries don't support query folding and therefore cannot take advantage of incremental refresh

Combining the data using merge will cut down on the use of functions like RELATED and RELATEDTABLE that return a related value from another table

You create multiple dashboards in Power BI Service and need to make sure users can see which dashboards contain Personally Identifiable Information (PII). What should you use?
- Senstitivity labels (Sensitivity labels provide a simple way for users to classify content in Power BI Service)

Line charts, with a single line, have a forecasting analytics option that can be enabled

Splitting out the time component from the date helps reduce the model size

Decomposition trees allow you to perform **exploratory** and **root cause** analysis

When a user is assigned to multiple roles, the RLS filters become additive and create a union between the filters

**The 50th percentile is also known as the median or middle value**

The key influencers visual shows the most important factors based on the fields provided

**Impact analysis** provides you the tools to understand how making changes to a dataset will impact downstream reports and dashboards

**bin**: You can set the bin size for numerical and time fields in Power BI Desktop. You can make bins for calculated columns, but not for measures. Use binning to right-size the data that Power BI Desktop displays.

**build** permission to dataset. For shared dataset, it is possible to grant 'build (report)' permission to recipients

You need to provide a user with the ability to add members to a workspace. The solution must use the principle of least privilege.Which role should you assign to the user?
- **Member** (Add **members** or others with lower permissions.)

ou have several reports and dashboards in a workspace. You need to grant all organizational users read access to a dashboard and several reports. Solution: You enable included in app for all assets. Does this meet the goal?
- No
- correct: 1, publish app. 2, grant access to certain groups.

You need to create a visualization that shows the relationship between Unit Price and Quantity Ordered. The solution must highlight orders that have a similar unit price and ordered quantity
- A Scattered plot of Quantity Ordered and Unit Price by item, Automatically find clusters

three columns: 
City 
Total Sales 
Occupation You need to create a key influencers visualization as 
- Total Sales, Occupation, City (analyzer, legend, influencer)

The indicator color for Total Sales will be based on % Growth to Last Year
- Background Color, Rules

You need to view the employees by region as quickly as possible. What should you do
- Create a new group on the state column and set the Group type to List

You have a Power BI tenant. You have reports that use financial datasets and are exported as PDF files. You need to ensure that the reports are encrypted. What should you implement?
- **Sensitivity labels**

The report uses data from a Microsoft SQL Server Analysis Services (SSAS) cube located on your company's internal network. You plan to publish the report to the Power BI Service.
- An On-premises data gateway

You have several reports and dashboards in a workspace. You need to grant all organizational users read access to a dashboard and several reports. Solution: You assign all the users the Viewer role to the workspace. Does this meet the goal
- No

Manage users that have access to the **app workspace**
- In the Microsoft 365, select **Members**
- (Workspace > ... > Members > (outlook.office365.com/..) > members/Add members)

You want to know which Teacher is responsible for which course
- Inner Join

when using Pivot feature, take care of the 'Aggregate Value Function'
- if you want to preserve duplicated values, you do not have to select the Sum option. (Don't Aggregate)

import **50 Microsoft Excel** files to Power BI Desktop
- Add a folder data source and use the Combine Files command

ColumnA presents several values starting with space;
ColumnB contains several non-printable characters.
- ColumnA: TRIM 
    ColumnB: CLEAN

In the Power Querry editor, select the text column you want to shape and the right click on them. This menu will appear:
- Transform > Trim/Clean/Length/...

split datatime before importing to power bi
- In order to improve our Power BI model performances, it is really important to work at the data source level. Among the different techniques available to optimize the modeling experience, there is the split between the date and time if they come from a single combined column

to replace null values with the date from the previous row
- command: Fill, and then Down

From the **Extract** menu, click Text After Delimiter
- Fist/Last Characters, Range, Text before/after delimiter, Text Between Delimiters

data model presents a huge list of queries that make it difficult to organize the transformation steps
- cteate a group of queries to classify the data-transformations

parameter
- M: Advance Query Editor > replace text by [varName] (the varName looks like Pythons)

 know which reports present a critical usage
- Request to the Power BI admin enabling usage metrics for content creators.

When you publish a Power BI Desktop file with a live connection to a tabular model to your Power BI site, an on-premises data gateway must be installed and configured by an administrator

standardize the creation and the sharing of Power BI content among the company units
- Deploy **pipelines tool**

Your organization plan to use the Power BI Service to get several visualizations from data stored in a custom application. The developers ask for pushing data into the Power BI Service from the custom app. How can you ensure this task
- Go to dev.powerbi.com/apps and **register an application**.

embed a report into the Microsoft SharePoint site
- *Publish* the report to the Power BI service - Obtain an *embed link* for SharePoint - Add a **webpart** to a page.

RLS can't restrict access to the layout of the report. With Apps, users can interact with the app content but can't modify it.

A Power BI user in your organization has published a report to the Web. The report contained sensitive data. What can you do to prevent the reports from being published on the Web?
- From the Power BI Admin portal, disable the Publish to web setting.

# 4.Administration settings in Microsoft PowerBI
manage the members that have access to the app workspace
- From the Office 365 Admin center, click Groups.

Your organization has a Microsoft SharePoint Online site named Enrollments where can access over 1000 users. After you have created a report in an app workspace on Power BI Service, you embed the report into a page on the Enrollments site by using the Power BI web part. You must ensure that all over the 1,000 users can view the report from the Enrollments Sharepoint site
- Configure the app workspace for **Premium capacity**.

You need to create a Power BI app workspace that will be accessible by 10,000 users. The dashboard contains sensitive data and you want that it will be updated every 1 hour. What should you do
- Configure the app worksapce for Premium capacity
- pro has a limit of 8 refresh daily

create a Machine Learning Model
- Get Power BI Premium - Create a Dataflow for the historical data - Add a Machine Learning Model.

Your customer owns a custom BI App based on PowerBI Embedded technology. He requests to scale up the capacity available for his custom BI App.
What do you need to change?
- **Pricing tier** from Azure Portal.

embed a report from the app workspace into a line-of-business application by using Power BI Embedded and APIs REST.
Which information should you provide to the application developers
- The application token and the report URL

add a specific user named User_01 as a member to a workspace
- Add-PowerBIWorkspaceUser - Scope Organization -/subscription ID/ -UserEmail Address user@data.com - AccessRight membe

# 5.Microsoft DAX language
create a goal for the number of sales made in the current year and set it as 10% higher than the number of sales made in the previous year
- GOAL = Calculate(Count('Sales'[SalesID]), PreviousYear('Date'[Date]))* 1.10

create a bar chart visualization to show the count of course enrollments by year that have an Enrollments Amount greater than 1,000.
- Larger enrollments = Calculate(Filter('FactcourseEnrollments','FactCourseEnrollments'[EnrollmentsAmount]>1000))






# [compare groups](https://docs.microsoft.com/en-us/microsoft-365/admin/create-groups/compare-groups?view=o365-worldwide)
- **Microsoft 365 groups** are used for collaboration between users, both inside and outside your company. They include collaboration services such as SharePoint and Planner.
- **Distribution groups** are used for sending email notifications to a group of people.
- **Security groups** are used for granting access to resources such as SharePoint sites.
- **Mail-enabled** security groups are used for granting access to resources such as SharePoint, and emailing notifications to those users.
- **Shared mailboxes** are used when multiple people need access to the same mailbox, such as a company information or support email address.

