# Trainer Efficacy Analysis 

This is an anlysis of trainee survey responses rating trainer efficacy for a non-profit group. 

First the good part: the trainers are reasonably consistent and have strong marks overall. The following is an ECDF plot, which represents the the percentage of the population that feel strongly confident they can impliment the training.

![ecdf](https://github.com/mhbw/tmc_git_files/blob/master/ecdf_agree_1.png)
As shown, the median of the population sits at 72% being highly confident in their ability to apply the material. 

That said, from an equity lense, there is room for improvement. Notably attendees that identify as People as Color feel 5% less prepared by the training lead by white trainers.

![poc_conf](https://github.com/mhbw/tmc_git_files/blob/master/poc_conf_poctrain.png)

<code>  Percentage of People of Color 'Strongly Agree' that they can implement the tools *when the trainer is white*:  69.83<br/>
Percentage when the trainer is a Person of Color:  74.86</code>

A T-test was performed on all data to evaluating confidence level. That test did not show a level of confidence or a p-value where a significant difference could be confirmed, likely in part due to the small sample size of the data. Testing aside the group should work with their white trainers to do better by attendees of color. 

<code>   stats.ttest_ind(training_data_npoc.PoCI_Strongly_Agree, training_data_poc.PoCI_Strongly_Agree)<br/>
Ttest_indResult(statistic=-0.77, pvalue=0.45)</code>

For this to be significant a P-value of 0.05 or lower, indicating 95% confidence level, is the typical standard. This p-value would indicate about a 55% confidence level, which is little better than a coinflip. 

### Staff Longevity 

Additionally,taking into acccount the longevity of staff, both PoC and White attendees feel less confident with older staff, (72 and 73% respectively) than with newer staff, who they feel about 73%-75% confident with. Interestingly the t-tests show that the racial groups do not have any difference in confidence level by tenure break out, which is to say, all demographics feel less confident with staff who have been on board for a longer time. 

![staff_conf](https://github.com/mhbw/tmc_git_files/blob/master/new_staff_conf_poctrain.png)
This number is also not statistically significant, but given the consistancy should still be examined. 

Overall, the group should revisit their trainings, perhaps with the help of an outside group such as AEORTA who do excellent work helping organizations in the progressive space particularly in re-training the longer tenured staff to ensure more uniform application across attendees.

