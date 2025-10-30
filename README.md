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

The chart shows how coupon acceptance rates differ across various occupations. Overall, there’s a clear difference in how likely people are to accept a coupon depending on their specific occupation. People working in sales, legal, and building & maintenance jobs/positions had the highest acceptance rates, which means they were generally more open to using coupons. Students, managers, and those in acrchitecture & engineering showed moderate acceptance, staying around the middle range -- roughly 45–55%. On the other hand, retired individuals, and those in farming, fishing, forestry, and transportation & material moving jobs had the lowest acceptance rates, which suggests that coupons may not appeal as much to these groups/specific occuaptions. In the end, these results indicate that a person’s occupation and possibly their income level or lifestyle can influence how likely they are to accept a coupon.

<img width="2288" height="896" alt="image" src="https://github.com/user-attachments/assets/fccbc5f6-0519-4060-b3d7-d3a949ad58c7" />


A bit more analysis of our findings looked at acceptance rates by occupation, time, and passenger type which revealed obvious behavioral patterns among mid-priced restaurant coupon respondents: KEY FINDING: Overall, coupon acceptance is highest among employed adults traveling with a partner during daylight hours. This finding strongly suggesets that marketing to working couples on lunch or evening commutes offers the greatest conversion potential.

Occupation: As seen in the plot the highest coupon acceptance occurred among office & administrative support, computer & mathematical, and healthcare practitioners & technical professions around 55–60 %. Acceptance was notably lower among retired and business & financial groups, around 30–35 %.

Finding:  Targeting employed professionals during work-adjacent hours is most effective.
- Time of Day: Acceptance of coupons peaked at 10 AM around 60 %, followed by 2 PM aroud  53 % and 6 PM around 50 %. It then sharply declined in the evening time around 10 PM around less than 35%.

Finding: Distribute coupons mid-morning to mid-afternoon when users are planning meals or finishing work.

Passenger Context: Drivers with a partner accepted coupons most frequently around 63 %, compared to friends around 46 %, those alone around 42 %, and those with kids around 37 %.

Finding: Couples are the most receptive audience; family drivers the least.
Overall, coupon acceptance is highest among employed adults traveling with a partner during daylight hours, suggesting that marketing to working couples on lunch or evening commutes offers the greatest conversion potential.

<img width="1308" height="2156" alt="image" src="https://github.com/user-attachments/assets/5802f473-53a9-467e-b9a9-537f6c1c6dd3" />
