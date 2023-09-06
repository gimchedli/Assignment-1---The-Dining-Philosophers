# Assignment-1---The-Dining-Philosophers

## Assignment describtion

The Dining Philosophers is a well known problem in Computer Science that concerns concurrency. At a dining round table there are five philosophers who are supposed to have dinner. Philosophers are kind of special and while they have dinner, they either *eat* their food xor *think* about something. In order to be able to eat, they must get hold of two forks (the food is very special and cannot be handled with one fork). Unfortunately, there are only five forks at the table, each of them uniquely placed between two philosophers (the table is round, there is exactly one fork between any two philosophers -- each philosopher can only reach the two forks that are nearby). As a consequence, it is never the case that all philosophers can eat at the same time (max two at the time).  Eating is not limited by food quantity or stomach space (which are both assumed to be infinite). This problem is interesting because, depending on how they decide to pick the forks, the philosopher may reach a deadlock.

The goal of this project is to implement the dining philosophers problem in Go, with the following requirements:

- each fork must have its own thread (goroutine)

- each philosopher must have its own thread (goroutine)

- philosophers and forks must communicate with each other *only* by  using channels

- the system must be designed in a way that does no lead to a deadlock  (and each philosopher must eat at least 3 times).  Comment in the code why the system does not deadlock.

- a sequentialisation of the system (executing only one philosopher at  a time) is not acceptable. I.e., philosophers must be able to  request a fork at any time.

- philosophers must display (print on screen) any state change (eating  or thinking) during their execution.


## Solution 
