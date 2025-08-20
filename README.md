Berkeley Professional Certificate in ML/AI <br> Practical Application-1 (Module-5 / Assignment 5.1): <br> Will the Customer Accept the Coupon?

This project investigates customer behavior in response to different coupon offerings. Specifically, the goal is to apply concepts of Probability Distributions, Exploratory Data Analysis (EDA), and Visualization techniques to distinguish between customers who accepted a driving coupon and those who did not. The assignment focuses on applying data cleaning, statistical summarization, and visualization skills to better understand patterns of coupon acceptance, which has direct implications for marketing strategies, consumer engagement, and targeted promotions in real-world business settings.

Files, Folder, and Dataset Information

Repository Structure: The project is maintained under the repository "BerkeleyMLAI-Module5-Practical-Exercises". The folder structure is organized to separate raw data, processed outputs, and code artifacts.

Dataset: Link to Coupons Dataset

Contains 12,684 records and 26 attributes.

Columns represent customer demographics, lifestyle habits, driving information, and coupon interaction outcomes.

This dataset provides a balanced mix of categorical and numerical features suitable for both descriptive and inferential analysis.

Technology Stack:

Programming Language: Python

Libraries: pandas (data handling), numpy (numerical analysis), matplotlib & seaborn (visualizations)

Code Notebook: Analysis is documented in Jupyter Notebook, located in the Code folder: Link to Jupyter Notebook

Exploratory Data Analysis (EDA) and Dataset Inspection

The first step was to examine the dataset structure and attributes. A snapshot of the columns is shown below:


Handling Missing Data

A careful assessment revealed missing values in several columns.


The car attribute had a high percentage of missing data, making it unsuitable for inclusion in further analysis.

For the remaining attributes, missing values were imputed using the mode (most frequent value) strategy, which preserved the categorical structure of the dataset without significant information loss.

Duplicate Records

A total of 74 duplicate rows were detected and removed, leaving a final dataset size of 12,610 records for the core analysis.

Visual Analysis of General Patterns

Coupon Type Popularity
This visualization illustrates which coupons were most frequently offered and accepted.


Weather Preferences and Coupon Usage
An analysis of weather patterns suggests that environmental conditions may influence coupon redemption decisions.


Key Data Insights
Overall Acceptance

Out of the total observations, 7,157 customers (56.76%) accepted a coupon, indicating that more than half of participants responded positively to promotions.

Bar Coupon Acceptance Breakdown

The acceptance of Bar coupons displayed strong variation depending on demographic and behavioral factors:

Overall Bar coupon acceptance rate: 40.9%

Visitors to bars ≤3 times/month: 37.05%

Visitors to bars >3 times/month: 76.88%

Drivers aged >25 who visit bars: 69.52%

Drivers without children visiting bars ≥1 time/month: 71.32%

Bar-goers more than once/month, non-widowed, with no child passengers: 71.32%

Individuals under 30 visiting bars more than once/month: 72.17%

Low-income (<$50K) individuals frequenting cheap restaurants ≥4 times/month: 45.34%

Hypotheses on Bar Coupon Acceptance

Based on EDA, the following hypotheses can be proposed:

Age Effect: Younger adults (particularly <30 years) who frequently socialize are significantly more inclined to accept Bar coupons (~72%).

Economic Preferences: Lower-income individuals exhibit a stronger preference for cost-effective options, such as cheap restaurants or discounted bars.

Lifestyle Patterns: Drivers without children and those who identify as more socially active show higher coupon acceptance rates.

Behavioral Frequency: Coupon acceptance increases with the frequency of visits—regular customers are more open to deals.

Occupational Influence: Customers not employed in fishing, farming, or forestry demonstrated higher acceptance (~56%), possibly tied to lifestyle differences.

Age 25+ Decline: Acceptance among drivers aged >25 decreases considerably (~33%), suggesting a generational difference in responsiveness to promotional offers.

Independent Analysis – Coffee House Coupon Acceptance

A deeper dive was conducted into Coffee House coupon acceptance patterns, exploring correlations with demographic and lifestyle attributes.

A. Coffee House Coupons & Age
Acceptance is highest among individuals in their 20s, highlighting generational differences in café culture and socialization habits.


B. Coffee House Coupons & Occupation/Education
People with no/some college education or those unemployed show higher acceptance rates, indicating coffee houses may serve as affordable social hubs. Students also prominently accept these coupons.


C. Coffee House Coupons & Marital Status
Divorced and widowed individuals exhibit lower coupon acceptance, possibly due to different social engagement patterns.


D. Coffee House Coupons & Education Level
Professionals with higher education backgrounds are less likely to redeem coffee house coupons, possibly reflecting different preferences (e.g., fine dining or alternate leisure activities).


Recommendations & Next Steps

To build on these findings, several next steps are proposed:

Feature Simplification: Streamline the dataset to reduce redundancy and improve model performance.

Expanded Variable Analysis: Incorporate underutilized attributes (e.g., Destination, Location, Direction, Time of Day, Weather) to uncover deeper behavioral insights.

External Data Integration: Merge with related datasets, such as customer income distributions or regional lifestyle trends, to provide broader context.

Predictive Modeling: Develop classification models (e.g., logistic regression, decision trees, random forests) to predict coupon acceptance likelihood.

Business Application: Translate findings into actionable marketing strategies—such as targeted promotions for younger adults, tailored bar offers for frequent socializers, and coffee house deals for students.
