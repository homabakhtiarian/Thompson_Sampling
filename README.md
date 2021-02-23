# Thompson Sampling

### Dataset
The dataset consists of 10000 rows and 10 columns that represent different ads. We're going to show ads to each of these users.
And because this dataset is a simulation Well we know for each of them on which ad they're going to click.

### What is Thompson Sampling?
Thompson Sampling is an algorithm for choosing the actions that address the exploration-exploitation dilemma in multi-armed bandit problem.
Actions are performed several times and are called exploration. 
It uses training information that evaluates the actions taken rather than instructs by giving correct actions. 
This is what creates the need for active exploration, for an explicit trial-and-error search for good behaviour. 
Based on the results of those actions, rewards (1) or penalties (0) are given for that action to the machine. 
Further actions are performed in order to maximize the reward that may improve future performance. 
Suppose a robot has to pick several cans and put in a container. 
Each time it puts the can to the container, it will memorize the steps followed and train itself to perform the task with better speed and precision (reward). 
If the Robot is not able to put the can in the container, it will not memorize that procedure (hence speed and performance will not improve) and will be considered as a penalty.

Thompson Sampling has an advantage of the tendency to decrease the search as we get more and more information, 
which mimics the desirable trade-off in the problem, where we want as much information as possible in fewer searches. 
Hence, this Algorithm has a tendency to be more “search-oriented” when we have fewer data and less “search-oriented” when we have a lot of data.
