Practical Application 1: Will the Customer Accept the Coupon?
Project: A mid-priced restaurant wants to increase customer traffic using targeted coupon campaigns.  This analysis identifies who, when, and where customers are most likely to accept coupons for similar mid-priced dining experiences.

Data cleaning -- 
I first dropped column car due to inconsistent and sparse entries.
I then filled missing values in _Bar, CoffeeHouse, CarryAway, RestaurantLessThan20, and Restaurant20To50_ with 'never'.
Filtered the dataset to focus on coupons labeled _Restaurant(20-50)_.
Verified data types, nulls, and distributions using pandas methods.

Exploratory Data Analysis (EDA) & Visualizations (5 pts)

Key variables influencing acceptance were explored using Seaborn bar plots:
  Feature	Visualization Goal
  Occupation	Identify which professions accept coupons more often  
  Time	Determine most effective times of day
  Weather & Temperature	Assess external conditions influencing decisions  
  Passenger	Examine social context of driving scenarios
  Restaurant Frequency	Compare loyalty vs coupon response




Findings: Coupon Acceptance by Occupation

The chart shows how coupon acceptance rates differ across various occupations. Overall, there’s a clear difference in how likely people are to accept a coupon depending on their job type. People working in Sales, Legal, and Building & Maintenance jobs had the highest acceptance rates, meaning they were generally more open to using coupons. Students, Managers, and those in Architecture & Engineering showed moderate acceptance, staying around the middle range (roughly 45–55%). On the other hand, Retired individuals, and those in Farming, Fishing, Forestry, and Transportation & Material Moving jobs had the lowest acceptance rates, suggesting that coupons may not appeal as much to these groups. These results indicate that a person’s occupation—and possibly their income level or lifestyle—can influence how likely they are to accept a coupon.

<img width="2288" height="896" alt="image" src="https://github.com/user-attachments/assets/fccbc5f6-0519-4060-b3d7-d3a949ad58c7" />


