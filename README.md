# Reinforcement Learning-based autonomous driving agent

<div align="center">
  <a href="https://deepwiki.com/SXV357/RL-Autonomous-Driving-Agent">
    <img src="https://img.shields.io/badge/DeepWiki-Ask-blue" alt="Ask DeepWiki">
  </a>
</div>
<br />

The overall aim of this project was to teach a reinforcement learning agent to drive by itself by learning from its surroundings, and using that information to make a decision that will lead to the best reward. Some considerations going into this project were how automation can help ensure personal/environmental safety, prevent motor vehicle accidents, devastation of impaired driving, drugged driving, and unbelted vehicle occupants.

The project is split into 3 notebooks:
  1. **Part 1 - Intro to Driving:** Set up the OpenAI Gym `CarRacing-v0` environment, implement the reinforcement learning loop, and write hand-coded driving policies that let the agent distinguish the road from its surroundings.
  2. **Part 2 - Behavioural Cloning:** Train a convolutional neural network on recorded driving data to predict the best action for every frame, and use it as the agent's driving policy.
  3. **Part 3 - DQN:** Look at exploration vs exploitation in terms of q-learning (starting with Blackjack), implement the Epsilon Greedy Policy, and train a Deep Q-Learning model that outputs a q-value for each of our actions. To wrap it up, we tweak the environment to penalize the agent, visualize loss graphs to estimate the extent to which the agent is able to safely navigate the environment, and run our model on a couple of simulations to see how well it performs.

The environment in which we will be training our agent has certain components and they are:
  1. States/observation - The current position of the agent or what the agent sees when it's in the environment
  2. Actions - The possible actions the agent can take in a given state(traffic light)
  3. Rewards - A measure of how good taking a certain action in a state is
  
  ![](Images/Observations.png)

## Running

The notebooks are meant to be run in Google Colab. Each one downloads its own data (and, for Part 3, pre-trained checkpoints) in its first cells. They use OpenAI Gym (`CarRacing-v0`), TensorFlow/Keras, and keras-rl.

## Acknowledgements

Since this was a group project that didn't involve pushing changes to a central repository, but rather working in our individual Jupyter Notebooks, I would like to acknowledge other group members who worked with me on this - Sainik Ghosh, Rohan Abraham, Athulya Saravanakumar, Marc Donghun Yoo, and Valerie Eng. I would also like to acknowledge Dr. Kuan Chuen Wu, Lead Data Scientist at CatapultX (now Qortex), for guiding me and our group in completing this project. Last but not least, I would like to thank Inspirit AI for helping with the starter code on most of these notebooks, especially with pre-defined functions for loading in and pre-processing datasets, library import statements, and starter code for various algorithm implementations throughout each of the notebooks.
