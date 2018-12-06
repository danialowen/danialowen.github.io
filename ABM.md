# Agent Based Model

## What is an Agent Based Model?

Agent based Models (ABM) is commonly regarded as one of the most popular modelling techniques in the social and ecological sciences. ABMs help measure and understand the behaviour of individuals (regarded as Agents) under certain conditions at an individual level. These individuals or agents are then given an agency, which gives them the ability to behave in a certain way and allows each individual to interact with other Agents. 

ABMs are generally iterative models which essentially means that they are controlled by repeated processes until they stop by a control. There are generally two types of stopping controls for ABMs; count-controlled and condition-controlled. Where a count-controlled ABM will terminate after a set number of loops, regardless of the outcome, whereas, a condition-controlled ABM will stop when a certain condition of an outcome is met. 

The basic code elements of ABMs include the 'Model', 'Agent' and 'Environment'. The Environment in an ABM is regarded as the "world", it is where all of the agent's actions happen and usually represented as raster grid data. The agents themselves are the individuals that interact with the environment. The agents have a certain behaviour, based either mathematically or statistically, and can interact with other agents within the environment. Lastly, the Model code is used to set up the model and set the conditions such as the number of iterations.

### My Project

![ABM GIF](abm.gif)

My project is an assignment for a Masters module and includes creating an ABM displaying Sheep (the Agents) eating away at the grass (the Environment). Here is the link to my [GitHub Repsitory](https://github.com/danialowen/Leeds_Assignment_1) which includes the final ABM labelled "Assignment_1.py" along with the functions for the Agent class labelled as "agentframework.py".

