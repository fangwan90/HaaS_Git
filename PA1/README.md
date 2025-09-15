https://github.com/fangwan90/HaaS/blob/main/prompt.ipynb

The car column contains only 108 data entries, comprising responses to a question on the type of car that the person drives. Since this variable will be used later, and does not affect the overall analysis, we leave the NaN values first. We assume that those who did not respond with their car models, do have a car, but did not want to share their car type. For accuracy, we filter away the rows for which the individual shared that they do not drive, albeit not significant to the overall analysis.  

Scooter and motorcycle                      22
Mazda5                                      22
do not drive                                22
crossover                                   21
Car that is too old to install Onstar :D    21

In general, without bias for any particular attributes, already more than 50% (56%) of respondents are willing to accept the coupon they were offered. Amongst coupon types, Coffee House coupons were the most common (almost 4000). From the dataset it seems like Coffee House coupons were used during the survey more. 

To dive deeper into the 2017 people who chose the bar coupon - around 41% of bar coupons were accepted, and amongst these, the acceptance rate for those who were already going to a bar more than 3 times a month, was some 40% higher (37% acceptance rate for those who went to a bar less than or equal to 3 times a month, but 77% for those who went to a bar more than 3 times a month). This meant that those who were already bar regulars, were more predisposed to accepting the bar coupon. 

After doing so, we can see that the acceptance rate for those who went to a bar more than once a month, and is >25yo, is about 70%, while those of others were about 34%. This suggests that legal age is a factor in those who are more likely to accept bar coupons - which makes sense, since they are unable to use the coupon if they are not of age. 

Filtering for acceptance rate between drivers who go to bars more than once a month and had passengers that were not a kid and had occupations other than farming, fishing, or forestry gives a result of about 71%, while those amongst others is about 30%, suggesting that this occupation field, or pax condition, may have higher predisposition for accepting bar coupons. 

Filtering again, for acceptance rates between those drivers who:
go to bars more than once a month, had passengers that were not a kid, and were not widowed OR
go to bars more than once a month and are under the age of 30 OR
go to cheap restaurants more than 4 times a month and income is less than 50K.
Yielded lower acceptance rates, suggesting that these factors - marital status, age beyond 30 vs just passing legal age, and income - were less determinant than the earlier two filters. 

Hence, to yield higher acceptance rates for bar coupons, one should consider: 

That the person is already a regular and goes to a bar >3 times a month 
That the person is of legal age and can go to a bar or 
That the person is not with a kid and had an occupation other than farming, fishing, or forestry. 

Looking now that those who were offered expensive restaurant coupons, the average acceptance rate is low, at only about 44%. 

if the person already goes to an expensive restaurant more than 4 times a month, it is slightly more likely to accept the coupon (64%) than if the person does not (42%). 
When it comes to income, there was no different in acceptance rate between those earning more than 50K vs less than 50k. When shifting this to 75k, the proportion did not change significantly, and remained comparable at 45% vs 44% - suggesting that income is not a determining factor. 
Age also does not seem deterministic whether above or below 40 years old. 
Highest match found was when the person was driving with a Partner in the passenger seat, and was single at that point in time, suggesting they were dating and likely that the person would be keen to impress (88%). This is slightly reduced if the person is merely driving with a Partner (63%) but may or may not be single at that point in time. 

With this, it suggests that success rate might be high for expensive restaurant coupons in cases when either, the person is already a regular patron of expensive restaurants, or if they were with a Partner in the car. 

Between these two cases, the data suggests that regardless of coupon types, regulars tend to accept the offered coupon type of restaurant types they frequent, and thus having such datapoint would allow one to more targettedly distribute such coupons. This is also why it makes most sense to simply distribute the coupons at the restaurants/cafes itself at the point of purchase/payment. 


