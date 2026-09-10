# 1.	Ask
Guiding questions
1.	What topic are you exploring?
Customers adoption of investment products.
2.	What is the problem you are trying to solve?
Increase conversion rates for investment products by reducing low effectiveness contacts and improving sales productivity.
3.	What metrics will you use to measure your data to achieve your objective? Who are the stakeholders?
Conversion rate and estimated potential revenue. Financial, marketing, investment and sales managers and executives.
4.	Who is your audience for this analysis and how does this affect your analysis process and presentation?
The audience is composed mainly of financial, marketing, investment and sales teams, so the results must be presented in a concise and visual presentation, highlighting the actions recommended.
5.	How will this data help your stakeholders make decisions?
This data will help managers to improve and set up marketing campaigns to reach the right customers and obtain better results.
Key tasks
It’s important to understand the problem and study early on so that you’re focused on your stakeholders’ needs.
•	Choose a case study
•	Identify the problem
•	Determine key stakeholders
•	Explore the data and establish metrics

2. Prepare
Guiding questions
1.	Where is your data located?
Dataset is the Bank Marketing Dataset from the UCI Machine Learning Repository
2.	How is the data organized?
Such data is related to direct marketing campaigns, based on phone calls, from a Portuguese banking institution.
3.	Are there issues with bias or credibility in this data? Does your data ROCCC?
4.5/5 ROCCC Assessment, since it’s partially current (the data was collected between May 2008 and November 2010). 
Potential limitations include geographic bias (single Portuguese banking institution), channel bias (telephone marketing only), historical bias (older data period), demographic bias (age, education, and occupation variables), and class imbalance in the target variable. These limitations should be acknowledged when interpreting results and making recommendations. 
4.	How are you addressing licensing, privacy, security, and accessibility?
The dataset is publicly distributed through the UCI Machine Learning Repository, which provides the dataset documentation, variable descriptions, and associated academic references. The dataset does not contain personally identifiable information. To ensure responsible data handling, the raw and cleaned datasets are stored separately and all transformations are documented.

5.	How did you verify the data’s integrity?
To verify data integrity, I reviewed the dataset documentation, checked for missing values, duplicates, inconsistencies, and formatting issues, and compared summary statistics with the original source documentation. All cleaning and transformation steps were documented, and both raw and cleaned datasets were maintained to ensure transparency and reproducibility.

6.	How does it help you answer your question?
This step is crucial to avoid wrong or imprecise insights or action recommendations. 
7.	Are there any problems with the data?
The dataset was revised and no major issues were found.
Key tasks
The prepare phase ensures that you have all the data you need for your analysis and that you have credible, useful data.
•	Collect data and store it appropriately
•	Identify how it’s organized
•	Sort and filter the data
•	Determine the credibility of the data


3. Process
Guiding questions
1.	What tools are you choosing and why?
Excel (initial exploration, pivot tables, filters, and quick charts) SQL (queries, aggregations, validations, and creation of summary tables), Python (Robust cleaning, statistical analysis, visualizations, and optional predictive modeling), Tableau (executive dashboard for the Share stage) and PowerPoint (final presentation with business storytelling).
2.	Have you ensured your data’s integrity?
Yes. Data integrity was verified by reviewing the official documentation provided with the Bank Marketing Dataset and comparing the dataset structure with the information published by the UCI Machine Learning Repository. I checked for missing values, duplicate records, incorrect data types, and inconsistencies in categorical variables. I also compared summary statistics and category distributions with the original documentation to confirm that the imported data accurately reflected the source data. The dataset contains real marketing campaign data from a Portuguese banking institution and includes detailed variable descriptions that support validation and quality checks.
3.	What steps have you taken to ensure that your data is clean?
Several data-cleaning procedures were performed before analysis:
•	Reviewed variable names and data types.
•	Checked for missing or null values.
•	Identified and removed duplicate records if present.
•	Standardized categorical values to ensure consistency.
•	Verified numerical variables for invalid values and potential outliers.
•	Created derived variables, such as age groups, to support segmentation analysis.
•	Ensured that all variables were correctly formatted for analysis in Excel, SQL, and Python.
These steps improved data consistency and reduced the risk of errors during analysis.
4.	How can you verify that your data is clean and ready to analyze?
The dataset was considered ready for analysis after completing several validation checks:
•	No critical missing values remained in key variables.
•	Data types matched the expected format for each field.
•	Categorical variables contain consistent labels.
•	Record counts remained consistent following cleaning activities.
•	Summary statistics and frequency distributions were reviewed for unusual values.
•	Random samples of records were inspected to verify accuracy after transformations.
These validation steps provided confidence that the dataset was complete, consistent, and suitable for analysis.
5.	Have you documented your cleaning process so you can review and share those results?
Yes. All data-cleaning activities were documented to ensure transparency and reproducibility. Documentation included:
•	The original source of the dataset.
•	Data-quality issues identified during inspection.
•	Cleaning and transformation steps performed.
•	Assumptions made during data preparation.
•	Validation procedures used to verify data quality.
•	The separation of raw data and cleaned data files.
Maintaining this documentation allows the analysis to be reviewed, replicated, and shared with stakeholders while preserving a clear audit trail of all modifications made to the dataset.
Key tasks
Now that you know your data is credible and relevant to your problem, you’ll need to clean it so that your analysis will be error-free.
•	Check the data for errors
•	Transform the data into the right type
•	Document the cleaning process
•	Choose your tools

4. Analyze
Guiding questions
1. How should you organize your data to perform analysis on it?
The data should be organized into a structured analytical dataset where each row represents a single customer interaction and each column represents a customer, financial, or campaign attribute. Variables were grouped into four logical categories:
•	Customer demographics (age, job, marital status, education)
•	Financial information (balance, loans, default status)
•	Campaign characteristics (contact type, campaign duration, number of contacts)
•	Campaign outcome (subscription: yes/no)
To facilitate analysis, additional variables such as age groups and conversion indicators were created. Aggregated tables and pivot tables were then developed to compare conversion rates across customer segments. The resulting structure allowed efficient analysis of relationships between customer characteristics and investment product adoption.
2. Has your data been properly formatted?
Yes. All variables were reviewed and formatted according to their appropriate data types.
•	Numerical variables were stored as numeric fields.
•	Categorical variables were standardized to ensure consistent labeling.
•	Missing values and duplicates were checked during the cleaning process.
•	Derived variables, such as age segments, were created to improve analytical clarity.
•	The final dataset was validated to ensure consistency between the cleaned data and the original source documentation.
This formatting ensured that the data was suitable for statistical analysis, visualization, and potential predictive modeling. 
3. What surprises did you discover in the data?
Several findings were unexpected.
First, customer demographics alone did not fully explain subscription behavior. Campaign-related variables appeared to have a substantial impact on the likelihood of a successful outcome.
Second, previous campaign outcomes showed a strong relationship with future subscription decisions. Customers who had positive interactions in previous campaigns appeared significantly more likely to subscribe again.
Another interesting finding was that customer age did not show a simple linear relationship with conversion. Certain age groups appeared to respond more positively than others, suggesting that customer behavior varies across life stages rather than increasing or decreasing uniformly with age. Research and analyses using this dataset frequently highlight the importance of previous campaign success, customer age segments, and campaign characteristics as influential variables.
4. What trends or relationships have you found in the data?
Several meaningful relationships emerged from the analysis:
•	Customers with successful prior campaign interactions demonstrated higher subscription rates.
•	Campaign characteristics, including contact frequency and communication method, appeared to influence conversion performance.
•	Certain occupations and education levels showed higher participation rates than others.
•	Age groups displayed different levels of responsiveness to financial product offers.
•	Financial indicators, such as account balance and existing financial relationships, appeared to be associated with subscription likelihood.
These trends suggest that both customer characteristics and campaign execution contribute to marketing success. Rather than relying on a single variable, conversion outcomes are influenced by a combination of demographic, financial, and behavioral factors.
5. How do these insights answer your question or solve the problem?
The analysis demonstrates that customer subscription behavior can be partially explained and predicted using demographic, financial, and campaign-related information.
By identifying customer segments with higher conversion rates, the client can:
•	Prioritize marketing efforts toward high-probability audiences.
•	Improve campaign efficiency by reducing contacts to lower-probability segments.
•	Develop more personalized communication strategies.
•	Allocate marketing resources more effectively.
•	Increase the likelihood of investment product adoption while reducing acquisition costs.
Therefore, the findings directly support the business objective of optimizing marketing campaigns and increasing revenue through more informed, data-driven customer targeting. The analysis confirms that customer segmentation can be used as a practical decision-making tool for improving financial product marketing performance. 
Key tasks
Now you’ll really put your data to work to uncover new insights and discover potential solutions to your problem!
•	Aggregate your data so it’s useful and accessible
•	Organize and format your data
•	Perform calculations
•	Identify trends and relationships

5. Share
Guiding questions
•	What story does your data tell?
•	How do your findings relate to your original question?
•	Who is your audience? What is the best way to communicate with them?
•	Can data visualization help you share your findings?
•	Is your presentation accessible to your audience?
Key tasks
During the share phase, you’ll tell a story using data and communicate your findings.
•	Determine the best way to share your findings
•	Create effective data visualizations
•	Present your findings
•	Ensure your work is accessible to your audience

6. Act
Guiding questions
•	What is your final conclusion based on your analysis?
•	How can you apply your insights?
•	Are there any next steps you or your stakeholders can take based on your findings?
•	Is there additional data you could use to expand on your findings?
•	How can you feature your case study in your portfolio?
Key tasks
After this, your case study will be complete. But you can use these steps again to help guide you through your analysis process.
•	Share next steps with your stakeholders
•	Determine if more data could give you new insights
•	Upload to your portfolio #
