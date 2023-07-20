# Reinforcement Learning Project
This repository contains the project for the UniTS reinforcement learning course A.Y. 2022-23. 
It was done in collaboration with [@alessimichele](https://github.com/alessimichele) and [@ElenaRivaroli](https://github.com/ElenaRivaroli).

[Here](...) you can find the final presentation slides.

# Flappy Bird solver
The goal is to teach an agent how to play the game flappy bird using the [text-flappy-bird-gym](https://gitlab-research.centralesupelec.fr/stergios.christodoulidis/text-flappy-bird-gym/-/tree/master).

The agent will have no knowledge of the environment but perfect observability of the states. As such it is phrased as a model-free reinforcement learning problem. 

Standard Reinforcement Learning techniques for policy control will be attempted and compared:
- [MC control](/MC_Control.ipynb)
- [SARSA](/SARSA.ipynb)
- [Expected SARSA](/E_SARSA.ipynb)
- [Q-Learning](/Q.ipynb)

# Results

For each methods, various set of hyperparameters were tested.
The resulting plots are stored in the [Plots](/Results/Plots/) folder for each hyperparameter configuration:
-   [MC Control](/Results/Plots/MC_plots)
-   [SARSA](/Results/Plots/SARSA_plots)
-   [Expected SARSA](/Results/Plots/Exp_SARSA_plots)
-   [Q-LEarning](/Results/Plots/Q_plots)

In [Summary](/Results/Summary/) folder are stored some statistics for each parameters configuration. The formatting of the files is described in [analysis](analysis.ipynb).

**Here are final results!**

![Agent playing before training](/Results/GIFs/before.gif)

![Agent playing after training](/Results/GIFs/after.gif)

### Some notes about the code
To implement this code we started from the one provided by the course tutor [Emanuele Panizon](https://www.ictp.it/member/emanuele-panizon). Moreover, chatGPT was used in the realisation of some small parts of the code, and this is noted accordingly in the code. 




