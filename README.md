# 276-Lab2

# Book Questions

Projects go wrong from lack of time over all other things combined.
This is because we are bad at estimating,
we confuse effort with progress,
schedule progress is badly monitored,
when schedule slippage is found man power is added which makes things worse

Programmers are often optimists because they're young.
This is not a good thing "this is the last bug etc" need to be more real
Mistakenly think things will take as long as they "should"
If our ideas are faulty we have bugs

Time vs. Workers for a perfectly partitionable task is that: Months go down and approach zero as Men go up and approach infinity
For a unpartitionable task (sequential constraints) Months stays at the same value as men go up (straight line)

Time vs workers when partitionable task requires communication has same curve as perfectly partitionable task but stops at a higher
month value

Time vs workers when the burden fo communication is made up of two parts, training and intercommunication. Each workder must be trained,
this cannot be partitioned so it varies linearly with worker count. Intercommunication increases n(n-1)/2. Or 3 workers requires 3x more than 2
and 4 requires 6x more than 2. These all result in a graph where months decrease until around 4-5 men and then months increase

Component debugging and system test give the most sequential constraints as the time required depends on the number and subtlty of errors
Because of optimism we think bugs are lower than they really are.

Scheduling sugggested: 1/3 planning, 1/6 coding, 1/4 component test and early system test, 1/4 system test, all components in # 
Note that the part easiest to estimate (coding) is given the smallest portion

Failure to have enough time to test and debug is really badly

Gutless estimating: being weak with estimates
Need to stiffen backbone (like chef cooking properly) and give info like bugs and estimates as time goes on

Suppose task assigned:
3 people 4 months (12 man-months estimated task)
If first part of task takes longer than anticipated (2 months) then manager must:
Assume only first part was mal estimated (add 2 men to make deadline), assume whole thing was mal estimated (add 6 men to make deadline),
just rechedule ortrim the task. In the first 2 cases insisting task could still be completed on time could be really bad.

Manager may assume that man go up month go down but does not consider training or communication
This is why we have Brook's law: Adding manpower to a late software project makes it later.





# Video Questions

currently @ 3:30 in video I go sleep now

describe the following git commands:

1. git checkout: Very safe, won't let your edit/ruin commit history
Can use a checkout commit to view code at a certain point in time, this is read only so commit history cannot be altered


2. git revert: Still safe, but a little less than checkout
Allows us to undo a particular commit, almost like it deletes it but it doesn't really however effect is still the same
in that it's like it never existed



3. git reset: Sort of unsafe, could ruin repo
Permanently takes you back in time to a certain commit, permanently deleting the commits after the time travel