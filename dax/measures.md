##Key DAX Measures

###Total Votes
'''DAX
Total Voted = CALCULATE(Sum('Voting Dash'[Voters]), 'Voting Dash'[Metric] = "Voted")

###Total Registered
'''DAX
Total Registered = CALCULATE(SUM('Voting Dash'[Voters]), 'Voting Dash'[Metric] = "Registered")

###Turnout Rate
'''DAX
Turnout Rate = DIVIDE([Total Voted], [Total Registered])

###Dropoff %
'''DAX
Dropoff % = 1 - [Turnout Rate] 
