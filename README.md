Practical Application 1: Will the Customer Accept the Coupon?
Project: A mid-priced restaurant wants to increase customer traffic using targeted coupon campaigns.  This analysis identifies who, when, and where customers are most likely to accept coupons for similar mid-priced dining experiences.


Dataset:: `coupons.csv` (UCI In-Vehicle Coupon Recommendation)  
Notebook:: [View Jupyter Notebook → practicalassignment1.ipynb](https://github.com/YourGitHubUsername/YourRepoName/blob/main/practicalassignment1.ipynb)

**Directory Structure**


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

The chart shows how coupon acceptance rates differ across various occupations. Overall, there’s a clear difference in how likely people are to accept a coupon depending on their specific occupation. People working in sales, legal, and building & maintenance jobs/positions had the highest acceptance rates, which means they were generally more open to using coupons. Students, managers, and those in acrchitecture & engineering showed moderate acceptance, staying around the middle range -- roughly 45–55%. On the other hand, retired individuals, and those in farming, fishing, forestry, and transportation & material moving jobs had the lowest acceptance rates, which suggests that coupons may not appeal as much to these groups/specific occuaptions. In the end, these results indicate that a person’s occupation and possibly their income level or lifestyle can influence how likely they are to accept a coupon.

<img width="2288" height="896" alt="image" src="https://github.com/user-attachments/assets/fccbc5f6-0519-4060-b3d7-d3a949ad58c7" />


A bit more analysis of our findings looked at acceptance rates by occupation, time, and passenger type which revealed obvious behavioral patterns among mid-priced restaurant coupon respondents: KEY FINDING: Overall, coupon acceptance is highest among employed adults traveling with a partner during daylight hours. This finding strongly suggesets that marketing to working couples on lunch or evening commutes offers the greatest conversion potential.

Occupation: As seen in the plot the highest coupon acceptance occurred among office & administrative support, computer & mathematical, and healthcare practitioners & technical professions around 55–60 %. Acceptance was notably lower among retired and business & financial groups, around 30–35 %.

Finding:  Targeting employed professionals during work-adjacent hours is most effective.
- Time of Day: Acceptance of coupons peaked at 10am around 60 %, followed by 2pm aroud  53 % and 6pm around 50 %. It then sharply declined in the evening time around 10pm around less than 35%.

Finding: Distribute coupons mid-morning to mid-afternoon when users are planning meals or finishing work.

Passenger Context: Drivers with a partner accepted coupons most frequently around 63 %, compared to friends around 46 %, those alone around 42 %, and those with kids around 37 %.

Finding: Couples are the most receptive audience; family drivers the least.


Overall, coupon acceptance is highest among employed adults traveling with a partner during daylight hours, suggesting that marketing to working couples on lunch or evening commutes offers the greatest conversion potential.

<img width="1308" height="2156" alt="image" src="https://github.com/user-attachments/assets/5802f473-53a9-467e-b9a9-537f6c1c6dd3" />

One more piece of analysis and findings regarding the time of day:

The following chart shows coupon acceptance at different times of day. Overall, coupon acceptance tends to be higher later in the day, especially around 6pm and 7am, where both coupon acceptance (orange bars) and total coupon offers are relatively high. 10pm also shows a large number of offers, but with a smaller share being accepted (as noted above w/ the sharp decline around 10pm). 10am and 2pm have fewer total offers and lower acceptance rates overall. These results suggest that people are more likely to accept coupons during commuting or meal-related hours, when they may already be out and more open to making a purchase.

<img width="1188" height="994" alt="image" src="https://github.com/user-attachments/assets/a2570fcb-042e-48a8-a9f8-476948b98b42" />


Next Steps and Recommendations

As someone still learning about data analysis and machine learning, my next step would be to collect more data on mid-priced restaurant coupons to make the results more complete and balanced. I would also like to try a basic predictive model—such as logistic regression or a simple decision tree—to see if it can help estimate which customers are more likely to accept a coupon. It might be interesting to test different expiration times and ways of sending coupons, like through an app, by email, or in person, to see which works best. Based on what I found in this analysis (main key finding), future coupon campaigns could focus on working adults with partners, especially during midday hours and on sunny days, since those conditions seemed to have higher acceptance rates.
