*Marcel Plakolb 3AHIF*
# Interprocess Communication

## Race Condition

###Describe with your own words: What is a race condition?
If there are multiple processes, the first one that enters a critical region is the only one that is allowed to execute the critical region. The others are "blocked" until the first thread leaves the crit. region.

## Arguments
###Why is it impossible to achieve Mutual Exclusion via disabling interrupts on a multi-core machine?
Because the threads can work simultaneously. That means it's impossible to ensure "Mutual Exclusion".

###Why is it dangerous to give user processes the power to disable interrupts?
If the process fails on a single core machine the computer isn't able to start another process.

##Peterson
###Play through the two scenarios of the handout of Peterson's solution. Document how it works.
If the first thread enters the crit. region it gets locked for the other thread via the shared variable loser and a bool[] that checks if the other process is inside critical region.

###Play through the scenario which makes the strict alternation approach fail. Document how it fails.
When two processes enter enter_region() at the simultaneously they might go in the while loop when the other process has not set the lock variable to true.

###What is the meaning of the variable loser in Peterson's solution? When does it have any effect?
If one thread is in a critical region and another process wants to enter, the shared variable llosder stops it from doing it.

###Extend the given functions such they can handle three processes.
