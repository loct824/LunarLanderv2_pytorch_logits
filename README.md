# LunarLanderv2_pytorch_logits

* This is a learning project applying REINFORCE (vanilla policy gradient) to the Gym Lunar Lander v2 environment
* The action space is 4-dimensional , the observation space is continuous.
* Refer to https://gymnasium.farama.org/environments/box2d/lunar_lander/ for environment details 
* The implementation here is minimal. RL framework classes (env, agent, policy) , neural network classes, data collection and training loop are all scripted in the same ipython notebook.
* This implementation takes references to TFAgent RL framework, in which environment's data are embedded inside a `TimeStep` class while the agent's action is embedded inside a `PolicyStep` class.
* DL framework is PyTorch, the optimization process (training loop) is done using manually coded formulas of REINFORCE algorithm, namely the loss function is reward-weighted entropy of action probabilities. 
* Anime video export is included at the end of the script.