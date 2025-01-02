To solve this problem with process mining, we needed to prepare the data before doing any conformance checking or statistic analysis.

So we filtered the data, so only student who took the image analysis course  into a new dataset and all the courses that has been taken after image analysis will be removed. After that we were splitting this data into two sub datasets, one with all the high performers and another one with the low performers. 

The purpose of this is to compare high performers and low performers. 

After preparing the given data, we had to make a model of the prerequisites of image analysis. Since the a student have to take the courses in a specific sequence, we had to work with a DCR graph for making a direction between the activities.

Then a conformance checking was done, which we will show later, that lead us to calculate the fitness on our business question.
And then we also did some analysis on the filtered student data with high and low performers to see which courses should be the actual prerequisites and if high and low performers have taken any prerequisites, which we also will show later on.
___________________________________
As mentioned before, we had to make our prerequisites model manually. But his model does not take the different groups of courses into account.

Cause as we see 
*click*
in kursusbasen, the prerequisites are splittet up into four groups giving the prerequisites a and or relation, that we will take into account in our fitness calculation, that we will show later. 