# Agent Based Model

## What is an Agent Based Model?

Agent based Models (ABM) is commonly regarded as one of the most popular modelling techniques in the social and ecological sciences. ABMs help measure and understand the behaviour of individuals (regarded as Agents) under certain conditions at an individual level. These individuals or agents are then given an agency, which gives them the ability to behave in a certain way and allows each individual to interact with other Agents. 

ABMs are generally iterative models which essentially means that they are controlled by repeated processes until they stop by a control. There are generally two types of stopping controls for ABMs; count-controlled and condition-controlled. Where a count-controlled ABM will terminate after a set number of loops, regardless of the outcome, whereas, a condition-controlled ABM will stop when a certain condition of an outcome is met. 

The basic code elements of ABMs include the 'Model', 'Agent' and 'Environment'. The Environment in an ABM is regarded as the "world", it is where all of the agent's actions happen and usually represented as raster grid data. The agents themselves are the individuals that interact with the environment. The agents have a certain behaviour, based either mathematically or statistically, and can interact with other agents within the environment. Lastly, the Model code is used to set up the model and set the conditions such as the number of iterations.

### My Project

![ABM GIF](abm.gif)

My project is an assignment for a Masters module and includes creating an ABM displaying Sheep (the Agents) eating away at the grass (the Environment). Here is the link to my [GitHub Repsitory](https://github.com/danialowen/Leeds_Assignment_1) which includes the final ABM labelled "Assignment_1.py" along with the functions for the Agent class labelled as "agentframework.py".

Above, is a GIF which demonstrates the final outcome of my condition-controlled ABM model. This model displays 10 individual Sheep (agents) eating away at the environment until each Sheep is full. This model is controlled by functions in the ["agentframework.py file"](https://github.com/danialowen/Leeds_Assignment_1) and the agents are made to:

- Move each sheep in a direction determined by the value of the random number produced. For example, each random number has a value ranging from 0 to 1 and a random number value greater than 0.5 moves the agent's x or y coordinates by +1, whereas, a random number value less than 0.5 moves each agent's x or y coordinates by -1.

- The sheep moves in a grid raster figure (100x100), thus, the move function had to include a "%100" remainder so that the sheep do not exceed the figure's boundaries.   

- Eat the environment (if the food is there) and stop when each of the sheep are full (has a food store of equal or above 5000). 

- Whilst eating the environment, the Sheep can interact with the other sheep. If two agents were positioned closer than the "neighbourhood" distance defined in the [final ABM](https://github.com/danialowen/Leeds_Assignment_1), then the two sheep would share their food equally.  


Whilst the functions for the Agents and the Environment are set, it is possible to modify some variables in the Model to examine the impact. For example, it is possible to modify the number of agents in the model, it is possible to modify the number of iterations per loop and possible to change the distance of the neighbourhood. It is interesting to see the impact of changing one or more of these variables and seeing what impact it has on the ABM. It is also possible to modify the condition on when the sheep are full, modifying this condition can determine how long the model will run for and how much the sheep will eat.
