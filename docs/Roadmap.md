[Back](../README.md)<br><br>
<h2 style="text-align:center;">How does a bike-share navigate speedy success.</h2>

## Ask
### Questions
- What is the problem you are trying to solve?
  - _My task is to Answer the question: How do annual members and casual riders use Cyclistic bikes differently?_
- How can your insights drive business decisions?
  - _My insights can guide the decisions for a campaign to convert the casual riders to members._

### Deliverable
- A clear statement of the business task
  - _The objective is to analyze bike share usage and customer behavior data to identify the most effective marketing strategies for converting casual riders into annual members. The goal is to increase the proportion of profitable, long term users._

## Prepare
### Questions
- Where is your data located?
  - _Data has been secured from the depository located at __https://divvy-tripdata.s3.amazonaws.com/index.html___
- How is the data organized?
  - _Data is organized in the csv format, separated by yearly quarters. The content of the files is organized in columns with data._
- Are there issues with bias or credibility in this data? Does your data ROCCC?
  - _Reliable - yes as in this scenario these data are internal._
  - _Original - yes as in this scenario these data are internal._
  - _Comprehensive - yes - the data are organized to well-named columns._
  - _Current - yes considering that for this scenario we would use the recent data._
  - _Cited - yes as in this scenario these data are internal._
- How are you addressing licensing, privacy, security, and accessibility?
  - _there are no issues with licensing as in this scenario these data are internal but the data itself were provided with the license, located at __https://divvybikes.com/data-license-agreement__._
  - _The data doesn't contain PII._
  - _No issue with security as the data were publicly available._
  - _Data are accessible in the depository located at __https://divvy-tripdata.s3.amazonaws.com/index.html__._
- How did you verify the data’s integrity?
  - _The data is from an internal source._
  - _The data contains small amount of duplicates and these were removed from the dataset._
  - _The first data set is missing about 5% of data in two columns of the user gender and user age._
  - _The second data set is missing only one datapoint but it has 210 zero-time rides form the HQ QR station._
- How does it help you answer your question?
  - _The data contain all the bike trips for a given period. These can be analyzed to understand how do annual members and casual riders use Cyclistic bikes differently._
- Are there any problems with the data?
  - _The data is well organized but some files have inconsistent column types._

### Deliverable
- A description of all data sources used
 data available from __https://divvy-tripdata.s3.amazonaws.com/index.html__
  - _Divvy\_Trips\_2019\_Q1 consecutively renamed as Cyclistic\_Trips\_2019\_Q1._
  - _Divvy\_Trips\_2019\_Q2 consecutively renamed as Cyclistic\_Trips\_2019\_Q2._
  - _Divvy\_Trips\_2019\_Q3 consecutively renamed as Cyclistic\_Trips\_2019\_Q3._
  - _Divvy\_Trips\_2019\_Q4 consecutively renamed as Cyclistic\_Trips\_2019\_Q4._
  - _Divvy\_Trips\_2020\_Q1 consecutively renamed as Cyclistic\_Trips\_2020\_Q1._

## Process
### Questions
- What tools are you choosing and why?
  - _I'm using Jupyter notebook with python because of ease of use of the Jupyter environment and Python because of the data quantity, which would be difficult to process in MS Excel._
- Have you ensured your data’s integrity?
  - _I have cleaned the data to ensure accuracy._
  - _I have used copies of DataFrames to ensure that there is no dependency on the order of sub-steps._
  - _Size of the dataset is large enough to not get influenced by removal of the duplicates or missing values and some missing values could be refilled from the rest of the data._
- What steps have you taken to ensure that your data is clean?
  - _I have unified the column naming between the datasets, made uniform values like gender or user type, made dtypes uniform, converted values to the right format, removed erroneous datapoints, and filled missing data from the rest of the datasets._
- How can you verify that your data is clean and ready to analyze?
  - _The data were described and compared with expected values._
- Have you documented your cleaning process so you can review and share those
results?
  - _Yes whole process is code written in the Jupyter notebook and can be recalculated at any time._

### Deliverable
- Documentation of any cleaning or manipulation of data.
  - _Whole process is written in the Jupyter notebook._

## Analyze
### Questions
- How should you organize your data to perform analysis on it?
  - _The data were organized in a DataFrame structure which is easily queryable with all tools I have used for this analysis._
- Has your data been properly formatted?
  - _The data has been ensured to have right format so no errors arise in the consecutive calculations._
- What surprises did you discover in the data?
  - _The different datasets had various naming conventions and some users were recorded as born in 1759._
  - _In the assignment it was stated that majority uses the service for leisure purpose however, from this analysis, the opposite was found._  
- What trends or relationships did you find in the data?
  - _I have found a clear distinction between casual and member users. which also divided them between leisure and commute users, respectively._
- How will these insights help answer your business questions?
  - _According to the patterns of the use of the service there are areas where it would be valuable to focus targeted marketing efforts._

### Deliverable
- A summary of your analysis
  - _The analysis highlights clear differences in usage patterns between member and casual users of the service. Members predominantly use the service on weekdays during commuting hours, indicating work-related travel. Casual users, in contrast, are more active on weekends and afternoons, reflecting leisure-oriented use. The user base is primarily male, though a notable proportion of female casual users remain unconverted. The largest user segment falls within the 30–40 age range, with many in this group also unconverted casual users. Trip durations differ, with members favoring shorter rides and casual users opting for longer trips, often over 30 minutes. Seasonal trends show increased casual usage in summer, while spatial data indicates casual users are concentrated around lakeside areas. These findings suggest opportunities for targeted marketing, seasonal promotions, and location-specific engagement strategies to drive membership conversions._
## Share
### Questions
- Were you able to answer the question of how annual members and casual riders use Cyclistic bikes differently?
  - _Yes._
- What story does your data tell?
  - _The majority of casual users use the service for leisure activity, which is connected with specific time periods and areas which could be a prime target for marketing efforts to convert them into members._ 
- How do your findings relate to your original question?
  - _My findings answer the original question._
- Who is your audience? What is the best way to communicate with them?
  - _This analysis is for a technical audience to showcase my approach of solving this task._
- Can data visualization help you share your findings?
  - _Yes, data visualizations are key to convey the findings._
- Is your presentation accessible to your audience?
  - _The presentation is hosted publicly under MIT license._

### Deliverable
- Supporting visualizations and key findings

## Act
### Questions
- What is your final conclusion based on your analysis?
  - _There are areas where it would be valuable to focus with the marketing efforts._
- How could your team and business apply your insights?
  - _They could use these findings to create targeted marketing strategies for both new and existing users._
- What next steps would you or your stakeholders take based on your findings?
  - _One could analyze data which would contain user tracking which could show the point at which the user converted. This could be also accomplished by creating pseudo users based on the similarity of the gathered data, if PII is not available._
  - _Stakeholders could utilize these findings to direct the marketing strategy._
- Is there additional data you could use to expand on your findings?
  - _Yes, additional data could be data connecting the same users together or zoning of the area to analyze how trips flow between zones._

### Deliverable
- Your top three recommendations based on your analysis
1. **_Implement Targeted Marketing and Conversion Campaigns for Female and Casual Users_**<br>
_Focus efforts on converting female and casual users, particularly within the 30–40 age group. Develop messaging that addresses their needs and emphasizes the benefits of membership, using data-driven insights to inform campaign timing and placement._

1. **_Launch Seasonal Promotions Aligned with Casual User Behavior_**<br>
_Introduce time-limited membership promotions during summer months when casual usage peaks. Emphasize value for longer rides and leisure-based travel, particularly in lakeside areas and other high-traffic casual zones._

1. **_Optimize Service Offerings Around Leisure Zones and Times_**<br>
_Enhance visibility and accessibility of services at lakeside and other high-use casual locations, especially during weekends and afternoons. Consider deploying pop-up kiosks, branded events, or trial ride programs during peak leisure hours to drive engagement and facilitate on-the-spot conversions._

<br><br>[Back](../README.md)