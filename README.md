# Model-Based-Reinforcement-Learning
The project consists of three classes: the GridWorld; the GridRules and the Agent.

The Gridworld class has two variables: two different tracks defined as 2D character numpy arrays. The two tracks correspond to the two configurations of the maze in the problem

The GridRules class defines the rules that govern how the agents moves in the maze. It takes two arguments: and instance of the GridWorld class; and an integer specifying the identity of the maze initially used in the GridWorld class.

Agent class defines the structure of the agent. It has two important functions: “run_episode_DaynaQ_ex” which implements the Alternate Method referenced in the problem set and “run_episode_DaynaQpve” which implements the DynaQ+ method. This functions return the optimal sequence of actions after each episode. This class takes three arguments: GridRules class; the value for epsilon; the value of the learning rate; the discount value; the initial values for the state-actions pairs, the number of planning steps, and the value of the constant for the bonus reward. The function “show_agent_sequence” displays the path traversed by the agent in the maze.

The notebook’s cells should be run in sequential order and the parameters such as epsilon; number of episodes, learning rate, planning steps, etc can be adjusted accordingly. The output of the entire program is a cmap of the paths taken by the agent and plot of the cumulative reward vs steps and the steps per episode vs the episodes
