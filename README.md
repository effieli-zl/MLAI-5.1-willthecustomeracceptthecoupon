# Will the Customer Accept the Coupon?
UC Berkeley MLAI | Required Assignment 5.1

## Jupyter Notebook
https://github.com/effieli-zl/MLAI-5.1-willthecustomeracceptthecoupon/blob/main/5.1_will_the_customer_accept_the_coupon.ipynb

## Key Findings

### Overall
- "Carry out & Take away" and "Restaurant(<20)" coupons have the highest acceptance rates.
- Drivers with no urgent destination are significantly more likely to accept coupons; drivers heading home have the lowest acceptance rate.
- Drivers are more likely to accept coupons when riding with friends, and less likely when riding with kids.
- Acceptance rates are higher on sunny days.
- Coupons with 1-day expiration have higher acceptance rates than 2-hour coupons.
- Drivers under 21 show high acceptance rates; rates decrease with age and slightly recover after 50.
- Drivers who regularly visit higher-end restaurants tend to have overall higher acceptance rates.

### Bar Coupons
- Regular bar-goers are more likely to accept bar coupons; frequent visitors over age 25 show even higher acceptance rates, possibly due to greater financial stability and flexibility.
- Drivers with kid passengers are less likely to accept bar coupons.
- Lower-income drivers who frequently visit cheap restaurants are less likely to accept bar coupons.

### Coffee House Coupons
- 10AM–2PM is the peak window for coffee coupon acceptance.
- Drivers aged 50+ have overall lower acceptance rates for coffee coupons.
- Younger age groups (below 21 to 30) show different patterns — acceptance rates don't drop significantly between 10AM and 2PM, and the 21–30 group even sees an increase.
- The 46–50 age group is the most time-sensitive: acceptance spikes from ~33% at 7AM to ~78% at 10AM, drops to ~36% by 6PM, then recovers to ~65% at 10PM.
- Time of day has a more consistent impact on coffee coupon acceptance for middle-aged groups (30–50) compared to younger and older groups.
- Time of day significantly impacts coffee coupon acceptance, and this effect varies considerably by age group, reflecting different lifestyle patterns across generations.
- By occupation, Healthcare Practitioners & Technical (76%) and Building & Grounds Cleaning & Maintenance (73%) show the highest acceptance rates, followed by Transportation & Material Moving, Healthcare Support, and Students (61–62%). Legal, Community & Social Services, and Sales & Related occupations show the lowest rates (<40%).
- Gender alone does not significantly impact acceptance rates; however, notable gender differences emerge within certain occupations — Installation Maintenance & Repair (F: 100% vs. M: 49%) and Construction & Extraction (F: 85% vs. M: 33%), likely reflecting the physical demands of these roles.
- Other lifestyle habits (bar visits, carry-away, cheaper restaurant visits) do not show a direct impact on coffee coupon acceptance; however, frequent visits to more expensive restaurants (Restaurant20To50) show a minor but consistent positive effect.
- Regular coffee house visits are the strongest lifestyle predictor of coffee coupon acceptance — acceptance rates increase significantly with visit frequency, with a diminishing rate of increase peaking at 4–8 visits per month, then slightly declining beyond that.

## Next Steps & Recommendations

### Overall
- Use destination context as a targeting signal — prioritize drivers with no urgent destination and avoid targeting drivers heading home if that data point is available, e.g. utilizing GPS data.
- Replace 1-day expiration coupons over 2-hour ones to improve acceptance rates.
- Avoid sending any coupon type when kid passengers are detected.

### Bar Coupons
- Target frequent bar-goers (more than once a month) over age 25 for highest ROI.
- Exclude drivers with kid passengers from bar coupon campaigns.
- De-prioritize low-income segments who frequently visit cheap restaurants — they show consistently lower interest.

### Coffee House Coupons
- Deploy coffee coupons primarily in the morning for peak acceptance.
- For age-based targeting, focus on under-30 and 26–50 groups; de-prioritize 50+.
- Prioritize Healthcare Practitioners, Building & Grounds, and Transportation workers by occupation.
- Cross-reference with coffee loyalty program data if available — regular coffee house visitors are the strongest predictor of acceptance.
- Gender alone is not a reliable targeting signal, but gender combined with occupation can surface high-value micro-segments.