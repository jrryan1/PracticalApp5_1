Goal: Determine which drivers are likely to accept a coupon delivered in the car.

Data: data/coupons.csv 
   Provided by UCI Machine Learning repository via Amazon Mechanical Turk survey

Images: images
   Visualizations build from the data
   
Code file: prompt.ipynb
   Jupiter notebood used to analyze the data file


Analysis:

Analysis of the data showed that overall acceptance rate for the coupons was 56.84%. Of the 5 coupons offered, Restaurants costly less than $20 per person and Carry out/Take away coupons had the highest returns with ~70% acceptance. See "couponAcceptRates.png".

Further breakdown into acceptance rates per time of day showed that coupons (except bar coupons) sent between 10am and 2pm had the highest overall acceptance rates. Some variation exists between coupon types (see images/timeofDayAcceptRates.png). Only Carry out & Take away coupons were above 70% at 10pm (75.9%). 

Further separating the data by gender shows that male drivers were ~2 to 6% more likely to accept the coupon (see images/genderAcceptRates with one exception. At 2pm, female drivers were 7.1% more likely to accept a coupon for Carry out/Take out. 

Separating the data by passengers, we found additional trends. Drivers alone at 10am were more likely to accept coupons for Carry out/Take away (92.1%) while drivers with their partners or friends were more likely to accept the same coupon at 6pm (93.8% and 91.3% respectively)

Weather and temperature had a direct impact on the responses. Rainy and Snowy days had low acceptance at 4.42% and 5.21% respectively. 
Comparitively, sunny days showed acceptance rate of 47.22%. Interestingly, this rate inceased to 59.25% while driving with friends

Additional analysis of the bar coupons showed a direct relationship between those that accepted the bar coupon and customers who already frequent bars. Specifically, drivers who frequent bars at least once per month are more likely (70%+) to accept a bar coupon. Further segmenting the data, drivers have an adult passenger or are under 30 most likely (71.8% and 72.2%) to accept the coupon.

On the other side, drivers who do not frequent bars (less than 1 per month) are least likely to accept bar coupons (33.5%) and drivers who have lower than 50K income and frequently (4+) visit low cost restaurants are also less likely to accept the bar coupon (43.8%).


Conclusion:
* Bar coupons had the lowest acceptance rate but were effective if driver frequents bars and was with a friend/partner or was under 30.
* Carry out/Take away coupons were the highest accepted coupons with rates regularly above 70%.
* Restaurants costing less than $20 per person were also high performers but did best between 10am and 6pm.
* Restaurants costing between $20 and $50 per person did see a spike of acceptance rates at 10am (~58%), 2pm (~50%) and 6pm (~48%).
* Coffee house coupons were ideally surved between 10am and 2pm with a focus on those traveling with kids.
