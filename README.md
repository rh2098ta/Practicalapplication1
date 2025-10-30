Practical Application 1: Will the Customer Accept the Coupon?
Project: A mid-priced restaurant wants to increase customer traffic using targeted coupon campaigns.  This analysis identifies who, when, and where customers are most likely to accept coupons for similar mid-priced dining experiences.

Data cleaning -- 
I first dropped column car due to inconsistent and sparse entries.
I then filled missing values in _Bar, CoffeeHouse, CarryAway, RestaurantLessThan20, and Restaurant20To50_ with 'never'.
Filtered the dataset to focus on coupons labeled _Restaurant(20-50)_.
Verified data types, nulls, and distributions using pandas methods.

Exploratory Data Analysis (EDA) & Visualizations 

Key variables influencing acceptance were explored using Seaborn bar plots:

  Occupation	Identify which professions accept coupons more often  
  Time	Determine most effective times of day
  Weather & Temperature	Assess external conditions influencing decisions  
  Passenger	Examine social context of driving scenarios
  Restaurant Frequency	Compare loyalty vs coupon response

Findings: Coupon Acceptance by Occupation

The chart shows how coupon acceptance rates differ across various occupations. Overall, there’s a clear difference in how likely people are to accept a coupon depending on their job type. People working in Sales, Legal, and Building & Maintenance jobs had the highest acceptance rates, meaning they were generally more open to using coupons. Students, Managers, and those in Architecture & Engineering showed moderate acceptance, staying around the middle range (roughly 45–55%). On the other hand, Retired individuals, and those in Farming, Fishing, Forestry, and Transportation & Material Moving jobs had the lowest acceptance rates, suggesting that coupons may not appeal as much to these groups. These results indicate that a person’s occupation—and possibly their income level or lifestyle—can influence how likely they are to accept a coupon.

<img width="2288" height="896" alt="image" src="https://github.com/user-attachments/assets/fccbc5f6-0519-4060-b3d7-d3a949ad58c7" />


Analysis of acceptance rates by occupation, time, and passenger type reveals clear behavioral patterns among mid-priced restaurant coupon respondents: KEY FINDING: Overall, coupon acceptance is highest among employed adults traveling with a partner during daylight hours, suggesting that marketing to working couples on lunch or evening commutes offers the greatest conversion potential.

Occupation: The highest coupon acceptance occurred among Office & Administrative Support, Computer & Mathematical, and Healthcare Practitioners & Technical professions (≈ 55–60 %). Acceptance was notably lower for Retired and Business & Financial groups (≈ 30–35 %).

- Targeting employed professionals during work-adjacent hours is most effective.
- Time of Day: Acceptance peaked at 10 AM (≈ 60 %), followed by 2 PM (≈ 53 %) and 6 PM (≈ 50 %), then declined sharply in the evening (10 PM < 35 %).

Distribute coupons mid-morning to mid-afternoon when users are planning meals or finishing work.

Passenger Context: Drivers with a partner accepted coupons most frequently (63 %), compared to friends (46 %), alone (42 %), and with kids (37 %).

Couples are the most receptive audience; family drivers the least.
Overall, coupon acceptance is highest among employed adults traveling with a partner during daylight hours, suggesting that marketing to working couples on lunch or evening commutes offers the greatest conversion potential.

<img width="1308" height="2156" alt="image" src="https://github.com/user-attachments/assets/5802f473-53a9-467e-b9a9-537f6c1c6dd3" />
