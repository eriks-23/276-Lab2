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


1. In your own words, summarize the chapter into 3-4 sentences.
The chapter explores the relationship between manpower and time taken to finish a project along with some other fallacies software engineers often have in regards to projects.
Many managers mistakenly believe adding individuals to a project will decrease the time for it to take to finish, in some cases this coul be true
such as if the task is "perfectly partionable". In reality however this is not usually the case as communication becomes more difficult as team members are added along with
the need to educate new members of a team. In cases like this a curve forms in which at a certain point adding team members results in the project actually taking longer than anticipated.
Other common mistakes include: unattainable deadlines, failure to allocate time to debug and being overly optimistic about time needed for debugging; mistaken ideas about these things
can lead to catastrophy in a project.

2. In your opinion, would adding more developers to a project that is running behind schedule be beneficial for the project? Explain your answer in 3-4 sentences, provide an quote from the chapter to support your answer.
I believe adding more developers to a late project is unlikely to be beneficial in most cases. The time sink of informing new team members and the added communication cost likely would make the project yield a later result.
As Brook's Law states: "Adding manpower to a late software project makes it later". The only case where I see adding more men to a late project could be of benefit is if the current team is not making any progress and added expertise could get them past a roadblock.

3.  Think back to a group project or teamwork experience you've had. Did you observe any parallels with the challenges described in "The Mythical Man-Month"? Explain your answer in 3-4 sentences and provide a specific example.
I had a group project last semester that I decided to start early as it was assigned at a time in between my midterms and finals. I created a basic prototype of the project and set up a layout for it. At this point I still didn't have
much of a solid communication plan with my group members so I kept working on the project until before I realized it I was almost finished. When I sent in what I had to my group they didn't need to add much to it for the project to be finished
however since they didn't understand all the libraries used etc. it took them longer to do the small amount left than it took me to do nearly the whole assignment by myself. I saw a pretty clear parallel with that project when reading this book. 

4. Given that "The Mythical Man-Month" was written decades ago, how do you think cultural and technological shifts since then might change or affirm Brooks' assertions? Explain your answer in 3-4 sentences and provide a specific example.
I think that the assertion made still holds fairly well today. Adding new members to a team in software development can still certainly be problematic even with new technology. An example of this is Call of Duty's Warzone gamemode.
New integrations put into the game new (guns, maps, character skins etc.) from each new Call of Duty game released would often result in bugs, poor balancing and more. At the time I was playing much of the community speculated that this was due to differing visions between the studios 
developing the games and poor communication when adapting multiplayer mechanics to the battle royale mode.

5. How do you plan on using the concepts from this book and applying it to your project in this course?
I plan to create a solid communicative base for the project so no member is left behind and has to play "catch-up" delaying the project.
I also plan to encourage my group members to allocate enough time to properly plan, test components and test the whole system. Hopefully we can
adopt a schedule similar to the one mentioned in the book of: 1/3 planning, 1/6 coding, 1/4 component test and early system test and 1/4 system test.

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