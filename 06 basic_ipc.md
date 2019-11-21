*Marcel Plakolb 3AHIF*
# Interprocess Communication

## Race Condition

###Describe with your own words: What is a race condition?
If there are multiple processes, the first one that enters a critical region is the only one that is allowed to execute the critical region. The others are "blocked" until the first thread leaves the crit. region.

## Arguments
###Why is it impossible to achieve Mutual Exclusion via disabling interrupts on a multi-core machine?
###Why is it dangerous to give user processes the power to disable interrupts?

## struct stat* statbuf
###Play through the two scenarios of the handout of Peterson's solution. Document how it works.
###Play through the scenario which makes the strict alternation approach fail. Document how it fails.
###What is the meaning of the variable loser in Peterson's solution? When does it have any effect?
###Extend the given functions such they can handle three processes.
